---
title: Bias
tags: [DRC]
date created: 星期四, 一月 18日 2024, 9:47:56 上午
date modified: 星期三, 二月 21日 2024, 2:35:55 下午
---

#DRC
# [[Edge]] Bias General
- pu.bias( layer_break, general_setting, special_setting)
```python
general_setting = {}
special_setting = []
rule1 = pu.EdgeSelection()
rule1.add_selection({'length': [0, 100], 'orientation': 'H'})
bias_table1 = {'bias': 15, 'bias_limit': 20}
rule1.anchor_special_setting(bias_table1)
special_setting.append(rule1)
```
- bias_table 中 bias 必须设置 bias_limit 不做设置也可