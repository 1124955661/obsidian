---
title: namedtuple
date created: 星期日, 一月 14日 2024, 7:23:34 早上
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

```python
>>> from collections import namedtuple
>>> Point = namedtuple('Point', ['x', 'y'])
>>> p = Point(1, 2)
>>> p.x
1
>>> p.y
2
```
`namedtuple`是一个函数，它用来创建一个自定义的`tuple`对象，并且规定了`tuple`元素的个数，并可以用属性而不是索引来引用`tuple`的某个元素。

这样一来，我们用`namedtuple`可以很方便地定义一种数据类型，它具备tuple的不变性，又可以根据属性来引用，使用十分方便。

可以验证创建的`Point`对象是`tuple`的一种子类：
```python
>>> isinstance(p, Point)
True
>>> isinstance(p, tuple)
True
```
