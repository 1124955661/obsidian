---
title: Job Manager
tags: [JobManager, job, Recipe, GUI]
date created: 星期二, 一月 2日 2024, 3:03:45 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#JobManager #job #Recipe #GUI 
# 相关信息
> [!info] 基础信息
> 	1. [[jmmaster]]：后台服务端log
> 	2. jmclient：客户端log
> 	3. [[jmviewer]]：前台用户操作
> 信息读取：{工作路径}/[[session_controller]]/[[session_controller#jobinfo.json|jobinfo.json]]
> 监控路径地址：用户在 [[jmviewer]].conf中设置的地址
## [[Jmmaster]]

[[jmmaster log]]
## [[Jmviewer]]

### Show Verbose Log
通过这个操作，查看当前job的报错信息。这个报错信息来源主要是[[session_controller#jobinfo.json|jobinfo.json]]，GUI是通过读取这个文件来获取信息的。
### Log
## PanGen Job 相关
### [[session_controller]]
主要是dp 和 job manager 模式的job，job 相关信息都会记录在这个文件夹中。
single 和 multiple 模式的 job 信息不会记录在这个之中。
## Slurm
### 基本命令
1. squeue：查看 slurm 队列的信息，并可查看job无法运行的原因
2. scontrol show job jobid：查看单个 job 的具体信息
3. sinfo：查看当前集群的信息
### Job 设置
```python
options['sbatch_setting'] = '-p gpu_48 --job-name=S2@CASEB -N 2 --ntasks-per-node=1 --cpus-per-task=2  --gres=gpu:1 --mem-per-cpus=10G'
```
 [[sbatch setting]] 
 [[pframe 中 if-else 的问题]]
--------------------------------------------------
## [[Job Manager PRD]]
# 实际问题
1. [[修改enable_execute_sessions|修改enable_execute_sessions]]
2. [[merge命令卡|merge 命令导致 session卡住]]
3. [[出现session_controller_temp]]
4. [[yaml文件报错]]
5. [[Remove Directory not empty]]
6. [[Permission Not enough to access monitor path]]
7. [[20240201 —— io_files_cksum]]