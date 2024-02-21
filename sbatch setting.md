---
title: sbatch setting
date created: 星期四, 一月 4日 2024, 10:54:41 上午
date modified: 星期三, 二月 21日 2024, 2:33:42 下午
---

1. -p：partition，设置提交分区
2. job-name：提交的 job 在slurm中显示的名字。
3. -N：节点数
4. ntasks-per-node：每个node 分配几个task（进程）
5. cpus-per-task：每个进程分配多少个cpu core数。
6. --gres=gpu：设置使用的GPU数量
7. mem-per-cpus：设置每个cpu core 可分配的memory。
>[!note] 注意事项
>	1. job 的 memory 上限，由 mem-per-cpus * cpu-per-task 决定，超过这个上限，job会abort。
>	2. 如果设置的memory数量超过当前服务器实际的物理上限，这个job 会卡在 slurm 队列中，无法提交，显示的原因是 resource。
