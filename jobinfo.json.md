---
title: jobinfo.json
tags: [file, system]
date created: 星期三, 一月 10日 2024, 4:59:01 下午
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

#file #system 
记录了当前job的状态信息，包括session相关信息。
## Job信息
- start time： job 开始时间
- first session start time
- job status：
- reason：报错原因
- current session：当前运行的session
- current session id：当前 session 在slurm 中的 jobid 号
- current session status
- session name：该job内的session list
## Session 信息
- session name:
- id:
- submit time: session 提交时间
- start time：开始运行的时间
- end time：
- percent complete：进度
- status
- option：是否被保存。（false 表示为被保存）