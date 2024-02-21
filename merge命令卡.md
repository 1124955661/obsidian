---
title: merge命令卡
tags: [问题, system]
date created: 星期二, 一月 2日 2024, 5:37:23 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#问题 #system
# 情形

worker 起来了，有log，log中的 上一个 **read command end** 到下一个 **read command begin** 之间的间隔很长
# 解决步骤

注释掉 merge 命令
