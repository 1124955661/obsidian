---
title: contextlib
date created: 2024-03-09T9:31:04
date modified: 2024-03-18T10:27:44
---

在Python中，读写文件这样的资源要特别注意，必须在使用完毕后正确关闭它们。正确关闭文件资源的一个方法是使用<font color=orange >`try...finally`</font>:

```python
try:
    f = open('/path/to/file', 'r')
    f.read()
finally:
    if f:
        f.close()
```
