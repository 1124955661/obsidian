---
title: 修改enable_execute_sessions
tags: [system, job, pframe]
date created: 星期二, 一月 2日 2024, 5:52:24 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#system #job #pframe
### 情形
1. 用户希望指定跑某个 session，去工作路径下修改 .\_pframe.py 文件中的 enable_execute_sessions 这个 option
> [!note] 注意事项
>  1. 不能修改 perforce_sessions。否则，这个job会被识别为新的job。
>  2. 不能注释session，否则会报 **unable to obtain the specified name or id of session** 的错误。
>  3. 如果需要指定 *if-else内的session*，需要指定到前一个session。
# 解决步骤
1. 直接修改 .\_pframe.py 中的 **enable_execute_sessions** 这个 option 中的 session 范围。