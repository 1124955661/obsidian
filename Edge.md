# Edge selection

```python
rule = pu.EdgeSelection() 
rule.add_selection({'length': [0, 100], 'orientation': 'H'}) rule.set_reverse_valid(True) 
rule.anchor_mark('A')  //打mark
```
# Edge type
1. jog **优先判断**
    - _**jogside 在jog边前后的两条边**_
        - 一般得满足 length ≥ min_jogside_len
    1. length ≤ jog_size
    2. **start_delta_angle = 270 or 90**
    3. **end_delta_angle = 270 or 90**
2. **lineend 再判断**
    - _**lineendside 在lineend前后的边**_
    1. length ≤ max_lineend_len
    2. previous1_length ≥ min_lineendside_len
    3. next1_length ≥ min_lineendside_len
    4. **start_delta_angle = 270**
    5. **end_delta_angle = 270**
3. **spaceend**
    - _**spaceendside 在spaceend前后的两条边**_
    1. length ≤ max_spaceend_len
    2. previous1_length ≥ min_spaceendside_len
    3. next1_length ≥ min_spaceendside_len
    4. **start_delta_angle = 90**
    5. **end_delta_angle = 90**
4. **run ：other 最后判断**
    1. **outcorner_vertex delta_angle = 270**
    2. **incorner_vertex delta_angle = 90**

1. 利用边的性质 写在这个函数内 _**rule.add_selection**_
    - length 边长
    - width/space 边的内外间距
    - angle
    - start_delta_angle/end_delta_angle 起始/终点的角度变化
    - orientation 朝向
    - start_vertex_type/end_vertex_type 起始/终点的类型
    - mark 标签
2. 通过表达式选取（和其他边的运算）_**rule.add_relation**_
    - Relation expression can be one or multiple 需要同时满足
    - Relation keywords supported:
        - properties : **length/width/space**
        - prefix: _**previous1/previous2/previous3/next1/next2/next3**_
    - _**Operators supported**_:
        - Comparison Operators:: _**==,≠,≥,≤,>,<**_
        - Unary Operators: - ,abs
        - Binary Operators: +,-,*,/,**
        - Multiple Operators: min,max
        - Other operators: ( . )
3. Edge Selection by Reference Layer 可以在同一层也可以是不同层 还可以是其他版图中的层