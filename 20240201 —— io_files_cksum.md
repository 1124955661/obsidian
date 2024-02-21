---
title: 20240201 —— io_files_cksum
tags: [bug, JobManager]
date created: 星期四, 二月 1日 2024, 2:18:28 下午
date modified: 星期三, 二月 21日 2024, 2:35:55 下午
---

#bug #JobManager 

# 情形

<font color=red size=5>GPU 环境</font> :
1. 在 pframe.py 中添加 enable_execute_session 和 perfoce_session 之后，无法成功提交 job。注释掉之后可以正常提交。
2. 经测试在本地是可以正常使用的

# 解决步骤

偶现问题，未知原因