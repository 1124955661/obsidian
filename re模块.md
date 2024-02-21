---
tags:
  - 正则
  - 编程
  - 字符串
title: re模块
date created: 星期日, 一月 14日 2024, 7:23:34 早上
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

使用 前缀 r 可以不用考虑转义
```python
s = r'ABC\-001' 
```
```python
import re
re.match(r'\d{3}\-\d{3,8}$','010-12345')

```
[[切分字符串]]
