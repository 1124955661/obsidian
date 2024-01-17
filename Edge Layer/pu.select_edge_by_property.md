#edge #EdgeLayer 
```python
rule = pu.EdgeSelection()
rule.add_selection({'length':[0,100]})
rule.set_reverse_valid(True)  # 

pu.select_edge_by_property(layer，select_rules) # 基于属性选择 edge，这条命令返回的结果是 edge

```
1. 先利用 pu.EdgeSelection()，基于属性设定 rule
2. 再根据一些特定的rule，进行 edge的 选择
select_rule: 
	1. Lenth
	2. Angle
	3. delta angle
	4. vertex
	5. orientation
	6. location，用于规定edge的相对位置，相邻两条边 ^a8e2f6

以上6种，property在使用的时候，均需要以字典的形式写出

支持反转。把 set_reverse_valid 的值设置为真的时候，选择规则中涉及到edge方向的设置会反转，如start vertex的值将会变成 end vertex的值，end vertex的值将会变成start vertex的值，previous1和next1也会互换。随后选择操作会基于反转后的规则再执行一次。 ^85b226

