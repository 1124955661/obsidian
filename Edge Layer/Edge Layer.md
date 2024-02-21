---
aliases:
title: Edge Layer
tags: [EdgeLayer, DRC, Recipe]
date created: 星期二, 十二月 19日 2023, 11:25:36 上午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#EdgeLayer #DRC #Recipe 
## Geometry
1. 方向性：
	假设你沿着[[edge]]行走，如果你的右侧为[[polygon]]，左侧为空的space，那么你行走的方向就是该条[[edge]]的方向。
2. 角度：
	沿着逆时针计算出基准线方向与[[edge]]方向之间的夹角，即可获得该[[edge]]的角度。对于两条相邻的[[edge]]，后一条边的角度减去前一条边的角度，即可获得后一条边的起点夹角start delta angle，同时它也是前一条边的终点夹角end delta angle。

## 什么是[[Edge]] Layer

1. [[Edge]] layer 与 [[Polygon]] layer 不同，可以把它视为一段 width 为 0 的 [[polygon]]。
2. [[Edge]] layer 也不同于 mark，[[edge]] layer 上一个可实际操作的 layer 对象，可以像[[polygon]] layer一样作为命令的input layer，而mark可以视为[[polygon]] layer的一种property，是依附于[[polygon]] layer而存在的，无法单独对mark做write，而是需要对其所属的[[polygon]] layer进行write。
3. [[Edge]] layer可以直接用.write()写出至 GDS/OAS文件中，并用GUI界面直接独立地查看。

## [[Edge]] 的选择
[[pu.select_edge_by_property|根据edge属性选择]]
[[pu.select_edge_by_relation|根据edge关系选择]]
[[dimensional Check|dimensional check]]
# 交互操作
[[edge]] 和 [[polygon]] 的交互操作。如何根据 [[edge]] layer 生成 [[polygon]]，以及如何根据 [[edge]] layer 选择[[polygon]]。
主要通过两个命令：
[[pu.edge_expansion()]]
[[pu.select_polygon_by_relation]]




