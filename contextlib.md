---
title: contextlib
date created: 星期日, 二月 4日 2024, 9:11:33 晚上
date modified: 星期三, 二月 21日 2024, 2:33:43 下午
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



