---
tags:
  - JobManager
  - job
  - WorkFlow
---
# Job Manager Work Flow
## 登入系统
1. 输入账号密码登入系统

## 准备阶段

### [[Job Manager 文件相关]]
- excel 文件，recipe，

### 导入 Job
1. 点击 Import 按钮
2. 选择 excel 文件，recipe，work path， output path
3. 输入 资源情况 worker node，worker count，gpu
导入之后，直接进入 job list
## Monitor 界面
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
### button
1. Submit：选中 job 之后，点击 submit 按钮提交
2. Delete：删除选中的记录
3. Kill：kill running的job
4. Select：quick select 功能

## queue 界面
- 当 Job submit 之后，会被提交进队列中，并把队列信息显示在GUI上
- 提供4个按钮用于调整 job 的顺序
- 提供搜索功能
## 资源查看
### resource
当前为显示 node 节点的资源情况，——思考是否需要更换成只显示 partition 的资源。（GUI中添加可以指定提交partition的功能）
### realtime resource 
实时显示 job 的资源使用情况。