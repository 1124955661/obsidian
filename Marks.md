---
title: Marks
date created: 星期五, 一月 5日 2024, 2:36:29 下午
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

对edge 或是 polygon 打mark，添加别名。
- Mark by Property
    - anchor_mark( ) 添加标记名
    - pu.mark_by_property( layer , rules)
- Mark by Relation
    - pu.mark_by_relation(layer, reference_layer, relation, mark , operation) tip： operation为relation满足的关系是and 还是 or(default)
    - relation with polygon：inside / outside / collinear / point / touch