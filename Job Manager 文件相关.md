---
title: Job Manager 文件相关
date created: 星期五, 一月 26日 2024, 10:32:02 上午
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

#### Excel 文件
1. PROJECT NAME: 
2. INPUT_GDS_PATH:
3. INPUT_GDS
4. customization: 用户自定义的参数
>[!note]
> >上述三个变量均需要大写 —— 可以讨论
> >INPUT_GDS_PATH 和 INPUT_GDS 两列需要连在一起
### Recipe
1. 在jmviewer.conf 中设置 recipe path
2. script 的命名是 xxx_template.py —— 这个需要修改
	1. 导入时不需要填写 xxx 这个关键字去fetch 脚本
#### Update 功能
1. 需要在 script 中设定 update 的区域
```python 
# JM START
...
# JM END 
```