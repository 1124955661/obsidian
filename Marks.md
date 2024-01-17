对edge 或是 polygon 打mark，添加别名。
- Mark by Property
    - anchor_mark( ) 添加标记名
    - pu.mark_by_property( layer , rules)
- Mark by Relation
    - pu.mark_by_relation(layer, reference_layer, relation, mark , operation) tip： operation为relation满足的关系是and 还是 or(default)
    - relation with polygon：inside / outside / collinear / point / touch