---
title: pu.select_edge_by_relation
tags: [EdgeLayer, layer]
date created: 星期四, 十二月 28日 2023, 2:52:29 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#EdgeLayer #layer 
```python
pu.select_edge_by_relation(layer1,layer2,select_rules)
```
# 两层Layer的属性
它根据给定的relation从layer1中选择edge并输出为[[edge layer]]，也可对layer1和layer2进行布尔或的操作。
	1. 当select_rule中的relation keyword为布尔或时，layer1和layer2要求==均为[[edge layer]]==，即OR运算是对[[edge layer]]之间的OR。
	2. 当relation keyword为share、not share、touch、not touch时，layer1和layer2既可以是[[edge layer]]，也可以是polygon layer。
	3. 当relation keyword为inside、not inside、outside、not outside时，由于内外关系是相对于polygon而言的，所以layer1可以为[[edge layer]]或polygon layer，而layer2==必须是polygon layer==。
# Relation Keyword

1. OR指的是两个[[edge layer]]之间的boolean OR运算。
2. Share和not share将会从layer1中选择与layer2共线重合或者不共线重合的那一部分edge。
3. touch和not touch的选择方式是：一旦layer1中的edge的一部分与layer2中的edge有共线重合或者不共线重合的情况，那么整条edge将会被选中。
4. Inside和not inside是从layer1中选择在或者不在layer2的polygon内部的那部分edge。
5. outside和not outside是从layer1中选择在或者不在layer2的polygon外部的那部分edge。
注意在进行inside和outside的选择时，不包括inside collinear和outside collinear。

# Example
## OR
OR关键字会对输入的两层[[edge layer]]取或运算，如图中的[[edge layer]] A和[[edge layer]] B做OR后输出[[edge layer]] C，此时输出layer中的各条edge分别继承原来所在的[[edge layer]]中的property。当两个来自不同layer的edge反向共线并且存在重叠部分时，由于该重叠部分同时存在两个互相冲突的方向，所以OR运算的结果将会移除重叠部分，只保留非重叠部分。如下图所示，edge layerA和[[edge layer]] B反向共线，角度分别是180度和0度，且他们存在一段重合部分。当对他们做OR操作时，中间那部分重合的冲突边将被移除。

![[Pasted image 20231228151104.png]]
## share/not Share, touch/not touch
当relation参数为share和not share时，selection命令会自动做break操作，而touch和not touch则不会做break。以左图为例，要从layer A中选择相对于layer B是share关系的edge，由于来自不同layer的edge存在相交的情况，在交点处edge会被break成2段（_手势动作第__1__张图的__break__点_），被break后的edge的下面这部分edge segment与layer B的edge是共线重合的，能够被选出。对于touch关系来说，由于该段edge（_第二张图的左侧竖直长边_）与layerB的edge存在部分重合共线的情况，所以整条边都能被选中。
>[!note]
>要注意Share、not_share，touch、not_touch都是不包括point touch的，所以这里的point touch的情况不能被share和touch选出（_point touch__的位置_）。这与mark操作中的touch参数是有区别的，在mark操作中，touch指的是两条边point touch。
>
>此外选择出来的edge同样具有property，他们的property继承自他们原来所属的input layer，在这里即为layer A。

![[Pasted image 20231228152108.png]]

## (not)inside, (not) Outside
当relation参数为inside、not inside和outside、not outside时，selection命令也会自动做break操作，以左图为例，要从layer A中选择相对于layer B是inside关系的edge，此时这一条edge在该点处会被break成2段（_第__1__张图的__break__点_），被break后只有下面这段edge segment满足inside的条件进而被选出。同样的，在右图中也表示了在执行outside和not outside的选择时layerA的这两条竖直方向的边也被break，break后上面这两段满足outside的关系（_第__2__张图的__break__点_）。

要注意inside和outside是不包含共线重合的情况的，所以对于左图这条边（_inside collinear_）来说不属于inside，对于右图来说（_outside collinear__位置_）来说这里不属于outside。

此外选择出来的edge同样具有property，他们的property也继承自他们原来所属的input layer，在这里即为layer A。
![[Pasted image 20231228153505.png]]

