---
tags:
  - JobManager
  - job
  - WorkFlow
title: Job Manager Work Flow
date created: 星期四, 一月 25日 2024, 4:55:23 下午
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

# [Job Manager](Job%20Manager.md) Work Flow
## 登入系统
1. 输入账号密码登入系统

## 准备阶段

### [[Job Manager 文件相关]]
- excel 文件，recipe

### 导入 Job
1. 点击 Import 按钮
2. 选择 excel 文件，recipe，work path， output path
3. 输入 资源情况 worker node，worker count，gpu
导入之后，直接进入 job list
## Job 阶段
1. 选中Job 之后 点击 submit, Job 进入 queue 中排队。
	1. 可以在 job detail tab 中选中需要跑的 session 
	2. 可以调整 job 在队列中的顺序，用于管控job运行的顺序
2. 通过 status 和 user 列可以对job table 中进行筛选，快速选中相应的job。
3. 在实时资源显示界面可以查看当前slurm队列中的 job 的资源使用情况。
## After Job Done
- CKSUM：校验输出 GDS 的cksum的功能
- copy file to：用于 copy 工作路径下文件的功能。（应删除）
# 说明及需求改进
## Monitor 界面
## 导入界面
1. 取消 specified job 这一行，取消用户不必要的输入。
2. Worker node，Worker Count 合并为一行
3. 
### [[Job Manager —— job页面 | Job 页面]]
- Job 相关信息： project name，Job Nama，session，user，status
- 在 User 和 status 列，提供筛选功能
### [[Job Manager Job detail 页面|Job detail 页面 ]]
- 展示 Job 的详细信息，通过双击 Job 页面，可打开标签页
- Project, job, session count, start/end time, time cost, user, recipe update time, 
- worker node, worker count, recipe path, work path, output path, log
### Session 页面
展示详细的 session 信息
1. session name
2. status 
3. start time
4. end time
### 功能button
1. Submit：选中 job 之后，点击 submit 按钮提交
2. Delete：删除选中的记录
3. Kill：kill running的job
4. Update：Update recipe 
5. CKSUM：校验输出的 GDS 的CKSUM值
6. Select：quick select 功能

## Queue 界面
- 当 Job submit 之后，会被提交进队列中，并把队列信息显示在GUI上
- 提供4个按钮用于调整 job 的顺序
- 提供搜索功能
## 资源查看
### Resource
- 当前为显示 node 节点的资源情况，——思考是否需要更换成只显示 partition 的资源。（GUI中添加可以指定提交partition的功能）
### Realtime Resource
实时显示 job 的资源使用情况。