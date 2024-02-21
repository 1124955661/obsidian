---
title: Jmviewer
tags: [tool, GUI, JobManager]
date created: 星期四, 一月 4日 2024, 11:16:34 上午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#tool #GUI #JobManager

# 机制
1. GUI 刷新机制：
	1. 任何操作之后，刷新当前页面的时间变化，2s->4s->8s->10s
	2. 60s，刷新一次全表。
# 基础
Jmviewer 是 [[Job Manager]] 的 GUI。用户可以通过 jmviewer 去提交job 和 监控 job 的实际状态。
```xml
# jmviewer.conf jmviewer的配置文件
  1 <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
  2 <root>
  3     <jmviewer>
  4         <ip>0.0.0.0</ip> 
  5         <port>8105</port> 
  6         <share_output>1</share_output> 
  7         <cpu_gpu_ratio>2</cpu_gpu_ratio> 
  8         <job_save_path></job_save_path> 
  9         <recipe_path>/home/jiatao/work/job_manager/jobs</recipe_path> 
 10     </jmviewer>
 11 </root>

```

- ip：设置ip地址，用于连接到 [[jmmaster]]
- port：设置端口号，同上，用于连接到 [[jmmaster]]
- share_output：是否会覆盖之前的路径，1会覆盖，0会在路径下建立一个以时间戳命名的文件夹。
- cpu_gpu_ratio：cpu 和 gpu 的比率
- job_save_path: 设置 job 记录自动保存的位置，会创建一个 txt 文件保存执行结束的 job 的信息。
- recipe_path: 设置 recipe 的存放路径，GUI 在选择recipe时，