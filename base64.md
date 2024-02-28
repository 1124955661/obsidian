---
title: base64
date created: 星期三, 一月 17日 2024, 11:51:40 晚上
date modified: 星期三, 二月 28日 2024, 10:25:56 上午
---

Base64是一种用64个字符来表示任意二进制数据的方法。

### 原理

Base64的原理很简单，首先，准备一个包含64个字符的数组：

``` python
['A', 'B', 'C', ... 'a', 'b', 'c', ... '0', '1', ... '+', '/']
```

然后，对二进制数据进行处理，每3个字节一组，一共是`3x8=24`bit，划为4组，每组正好6个bit：
[cdn.liaoxuefeng.com/files/attachments/949444125467040](https://www.liaoxuefeng.com/files/attachments/949444125467040)
这样我们得到4个数字作为索引，然后查表，获得相应的4个字符，就是编码后的字符串。

所以，Base64编码会把3字节的二进制数据编码为4字节的文本数据，长度增加33%，好处是编码后的文本数据可以在邮件正文、网页等直接显示。

如果要编码的二进制数据不是3的倍数，最后会剩下1个或2个字节怎么办？Base64用`\x00`字节在末尾补足后，再在编码的末尾加上1个或2个 ==\=== , 表示补了多少字节, 解码的时候，会自动去掉。
Python内置的`base64`可以直接进行base64的编解码：

```python
>>> import base64
>>> base64.b64encode(b'binary\x00string')
b'YmluYXJ5AHN0cmluZw=='
>>> base64.b64decode(b'YmluYXJ5AHN0cmluZw==')
b'binary\x00string'
```

由于标准的Base64编码后可能出现字符`+`和`/`，在URL中就不能直接作为参数，所以又有一种"url safe"的base64编码，其实就是把字符`+`和`/`分别变成`-`和`_`：

```python
>>> base64.b64encode(b'i\xb7\x1d\xfb\xef\xff')
b'abcd++//'
>>> base64.urlsafe_b64encode(b'i\xb7\x1d\xfb\xef\xff')
b'abcd--__'
>>> base64.urlsafe_b64decode('abcd--__')
b'i\xb7\x1d\xfb\xef\xff'
```
