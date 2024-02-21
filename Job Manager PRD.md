---
title: Job Manager PRD
tags: [PRD, JobManager]
date created: 星期二, 一月 30日 2024, 11:45:22 中午
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

#PRD #JobManager 
## Improvement 记录
1. 支持 用户在 GUI 中 修改 worker count
2. 支持 多 partition 分区提交
	1. 用户手动指定提交的 partition 分区
	2. 通过查看 resource 界面中的 partition 资源情况，指定提交的分区
3. 不同的 partition 的 queue 应该是不同的，
	1. 可以轮询 queue 中的 job，并check 其提交的 partition 分区的内容，<font color=red>只需要维护一个队列</font>
	2. 针对不同的 partition 分区，设置不同的 queue。<font color=red>这样需要维护不同的队列</font>
	3. 