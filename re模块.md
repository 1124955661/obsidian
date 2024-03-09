---
tags:
  - 正则
  - 编程
  - 字符串
title: re模块
date created: 2024-03-09T9:31:04
date modified: 2024-03-09T9:31:39
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
