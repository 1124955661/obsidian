---
title: polygon containment
tags: [EdgeLayer, polygon]
date created: 星期二, 一月 2日 2024, 11:15:52 上午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#EdgeLayer #polygon 
# Define
在[[dimensional check]]中，假如一对pair edge满足selection rule，并且不被[[block edge]]所影响，它还需要满足多边形限制准则才能够实现输出。通俗地来说，polygon containment规定了不能穿过polygon去选择边的具体规则。

在single layer check时，如果mode为internal，只有当edge来自于同一个polygon时才会被选中，来自于不同polygon的pair edge结果将会被过滤。如下图1所示，尽管左侧的红色实线edge能够在constraint的范围内朝着internal的方向找到右侧的红色虚线edge，但是由于这一对edge并不属于同一个polygon，所以他们在标准结果中不能被输出。而在single check下的external mode不存在polygon Containment。

在bi-layer check中，如果mode为internal，对于满足selection rule的一对pair edge中的任意一个edge，它必须和另一个edge所属的polygon满足inside或者not collinear关系时，这一对pair edge才可以被选中并输出。如下图2所示，尽管左侧的红色实线edge能够在constraint的范围内朝着internal的方向找到右侧的红色虚线edge，但是这两条edge相对于另外一个polygon都是outside关系，所以他们在标准结果中不能被输出。

如果bi-layer check的mode为external，输入layer的edge相对于另一层必须满足not_outside和not outside collinear关系时才会参与操作。如下图三所示，左侧红色实线的edge相对于另一层layer是inside关系，此时尽管他与红色虚线的edge之间满足基本的selection rule，但由于不满足多边形限制准则，所以仍然不能被输出。

如果bi-layer check的mode为enclosure，来自于layer1的edge必须相对于layer2是inside和not collinear的关系，同时来自layer2的edge必须相对于layer1是not inside 和not inside collinear的关系。只有满足上述关系时，这两个edge才会才能与操作。如下图4所示，layer2中的红色虚线edge满足polygon containment的要求，但layer1中的红色实线edge相对于layer2是outside关系，所以即使这对edge满足基本的selection rule，他们也不会输出。
![[Pasted image 20240102111854.png]]