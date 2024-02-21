---
aliases:
title: dimensional Check
tags: [EdgeLayer, Recipe, function]
date created: 星期四, 十二月 28日 2023, 3:35:34 下午
date modified: 星期三, 二月 21日 2024, 2:35:55 下午
---

#EdgeLayer #Recipe #function
# 概念
在根据property进行选择时，并不建议使用width，space，enclosing，enclosed，self to reference width和self to reference space等property，这些property可以理解为通过测量一对 pair [[edge]]沿某个方向的相对距离，选择出符合要求的[[edge]]，[[edge]] selection的结果依赖于geometry setting中对query box的设置，即设置max_space，max_width，start_extend，end_extend的值。而对于一些特殊的边，需要重新改变query box。当涉及到这些property时建议使用dimensional check，它不需要手动设置geometry setting，可以在执行命令时灵活地改变query box。

为了方便快速理解，这里首先举几个用dimensional check实现上述property的例子。在dimensional check中，exterior 方向对应于朝着[[edge]]所在[[polygon]]的space的区域进行搜索，interior方向对应于朝着[[edge]]所在[[polygon]]的width的区域进行搜索。

根据前述定义，dimensional check规定了三个和搜索方向相关的关键字。internal关键字类似于with和self2reference _width，可由输入layer的个数具体控制是哪一个property。同样地，external关键字类似于space和self2reference_space。特别地，enclosure关键字描述了一对pair dge中一条[[edge]]朝着exterior方向，一条[[edge]]朝着interior方向的情况。此时对于上图左边这条边，可以参考enclosed property，同时也可以参考self2reference_space property，对于下图右边这条边则对应于enclosing和self2reference_width。
![[Pasted image 20231228155132.png]]


# 用法
```python
pu.dimensional_check( layer_one | [layer_one, layer_two], mode, constraint, metric, output, {extend, alter, projection, corner, intersection, polygon, reversal, shadow, shield})
```
1. 第一个参数: 输入层，可以是单层layer，将对自身做single layer check，或是多层layer（以list形式），输出的[[edge]] 默认来源于 layer 1，可以通过设置参数，输出layer 2中的[[edge]]。
2. Mode：决定了 dimensional check 的测量方向
	1. internal: 根据 interior 方向测量两条[[edge]]
	2. external：根据 exterior 方向测量两条[[edge]]
	3. enclosure：输入层必须为两层layer，其中layer 1朝着exterior方向，layer 2朝着interior方向。
3. constraint：规定沿着mode 方向的测量范围，以字符串形式写出，该字符串为 list 形式，这两个元素是非负整数，可通过中小括号，规定开闭区间。
4. metric：规定搜索区域的形状
	1. euclidean：即[[edge]]发出的搜索区域是Euclidean型，它在矩形搜索区域的基础上再以[[edge]]两侧端点为圆心额外延展出四分之一圆。
	2. square: 指搜索区域是在矩形搜索区域的基础上再沿着[[edge]]两侧端点额外延展出正方形。
	3. opposite：指矩形搜索区域
> [!note]
当使用opposite型的metric时，可以在options中指定extend的值，它可以控制矩形搜索区域沿着[[edge]]的两侧朝外延展的量。

![[Pasted image 20231228161700.png]]
5. output: 输出结果
	1. [[edge]]：输出被上述rule选择出来的[[edge]]
	2. inverse [[edge]]：输出不满足上述rule的[[edge]]，即反选
	3. region：输出满足 rule 的 pair [[edge]] 的端点连接而成的区域。
	4. extents：将region的结果延展成矩形
	5. centerline：输出region结果的中线，线宽默认是 2nm，该关键字可以写成一个字 典形式用以指定输出的线宽，同时该值必须大于 两个dbu。
	![[Pasted image 20231228164828.png]]
## Options：
1. extend：当 metric 为 opposite 时，让测量区域朝两侧延申一定值。
2. alter：应用于bi-layer的dimensional check，即输入为两层layer。一般来说，在bi-layer的dimensional check中默认输出layer1中满足要求的[[edge]]，如左图中的蓝色边，此时layer1为生成[[edge layer]]的基础layer。另一方面，这条蓝色的[[edge]]会和来自layer2的某一条[[edge]]组成一对pair [[edge]]，即右图中的蓝色斜边。当alter设置为1时，输出的结果会是pair [[edge]]中来自layer2的那条[[edge]]，此时layer2为生成[[edge layer]]的基础layer。![[Pasted image 20231228164929.png]]
3. projection：根据投影规则过滤输出的结果。project length：两边平行，或两边正交，为投影重叠部分的长度，no_project：两边垂直
	1. project：只有满足基本selection rule 并且有 project length的边才会输出，包括 project length 为0的情况。此外如果在一对pair [[edge]]中只是一条边朝着另一条边能够投影，而不是两条边能够互相投影，他们能被project关键字选中。
	2. {‘length‘：’\[min_value, max_value]'}：将基于selection rule 的结果输出具有一定投影长度的平行边，此时 pair [[edge]] 必须是平行的两条边，非平行边不会输出，且长度在区间范围内。
	3. no project：输出是 no project的边
4. corner：仅指90度的 corner
	1. C2C：包括45°和非45°，且 pair [[edge]]是 no project的
		1. {'C2C'：'D45'}：只有45°的 pair [[edge]]
		2. {'C2C'：'ND45'}：只有非45°的 pair [[edge]]
		3. {'C2C'：'collinear'}：考虑共线情况，同时也会选择 45°和非45°的情况。
	2. C2E：pair [[edge]] 之间存在projection，并且 corner的夹角是正交的
	3. AC：同时测量 C2C 和 C2E
	4. NC：AC的补集
5. intersection：相交边会额外的参与测量，三个参数可以同时使用。
	1. {'angle': '\[min_value,max_value]'}：规定mode方向下相交边之间的夹角范围，满足该范围的的相交边会额外参与测量，当不指定range时，默认是(0,180)
	2. point：[[edge]]相交在某一点的情况也会额外参与测量
	3. only：必须和 angle 和 point 联合使用。使用angle或者point关键字意味着在标准结果之外额外输出intersection的结果，而使用only关键字等同于过滤标准结果，只输出intersection的结果。
6. [[polygon]]：[[edge]]是否来自同一个 [[polygon]]
	- 只适用于 single layer 的 external check，该 option 将根据输出的 [[edge]] 是否来自同一个 [[polygon]] 实现对结果的过滤。如果 [[polygon]] 的值为 self，只有当 pair [[edge]] 来自同一个 [[polygon]] 时才会被输出，如果 [[polygon]] 的值为 diff，只有当 pair [[edge]] 来自不同的 [[polygon]] 时才会被输出。
7. reversal：[[edge]]相对于layer之间的关系（select_[[edge]]_by_releation)，只适用输入为2层layer的情况，使用这个option时，结果会额外输出满足相应情况的结果。
	1. inside_also：只可以在mode为 enclosure 或 external 的情况使用。使用该参数时，layer 1 中相对于 layer 2 为 inside 或 inside collinear 关系的边也会额外输出。
	2. outside_also：输出 layer 1 关于 layer 2 为 outside 和 outside collinear 的 [[edge]]。

	- 注意如果在使用reversal的同时，output参数指定为region，Extents或者centerline等，此时这些额外输出的边会朝着width的方向扩展1nm的宽度。
		![[Pasted image 20240102101745.png]]
8. shadow： ==Shadowing [[edge]]== 指的是能够完全或部分阻隔一对选中的 pair [[edge]] 之间视线的 [[edge]]。
	1. filter mode：0关闭，禁用该option，1开启。开启时，pair [[edge]] 形成的 region 中存在的哪些 shadowing [[edge]] 如果完全阻隔了 pair [[edge]] 之间的视线，那么这类pair [[edge]] 将会被过滤掉不被输出。==设置为 2 时==，如果只阻隔了部分，那么没有被阻隔的部分的 pair [[edge]] 将会输出。![[Pasted image 20240102102630.png]]
	2. {'count':'\[min,max\]'}：输出结果中，允许存在的showing的数量。
	3. {'shadow_layer': layer} : 只有来自指定层的 shadowing [[edge]] 有效
	- shadow option 和 shield: clear option 以及 projection：no project option 不能同时使用。并且 shadow option 中的相关定义对于相交边的情况并不生效。当metric是Euclidean和square 时，constraint中指定的min value必须写成0，即下限必须是>0或>=0。否则[[block edge]]的限制会失效。
9. shield：只适用于 bi-layer check，用于放宽测量行为的设定。
	1. block_[[edge]]：可以在 internal 和 enclosure check 中额外考虑 collinear 的情况。 inside collinear 的 [[edge]] 也会被纳入 internal check 的测量中， outside collinear 的 [[edge]] 被纳入 enclosure check 的测量中。 ^a37131
	2. clear：清除 [[block edge]] 和 [[polygon containment]] 对结果的影响。

