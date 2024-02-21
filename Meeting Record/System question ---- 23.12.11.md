---
title: System question ---- 23.12.11
date created: 星期一, 十二月 11日 2023, 2:03:50 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

# SMIC 问题
## Gearman 通信问题
1. [[poll timeout]] ，[[worker timeout]] 分别从5s->10s, 60s->180s
2. license 目前是2500
3. parent 和 worker 之间通信问题
	1. 目前通信延迟在40ms左右，相当于1s内，parent只能回25个worker的信息