---
title: slurm utilization question
tags: [bug]
date created: 星期二, 一月 30日 2024, 4:18:45 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#bug 
# 情形
slurm 中的 cpu 使用率低于 dp很多

# 原因
## Taskset

<font color=red size =5>结论</font>：slurm 中受限于申请的 core 的数量，使用率不高。dp 模式下 openmp 使用了更多的 core，使得使用率更高，

taskset 是一种限制 core 使用的设置，slurm 中相当于是自动设置了这个 taskset。
1. slurm 中是申请资源的逻辑，所以会受限于申请的 core 的数量。
2. dp 模式，由于打开了 <font color=red>openmp</font>，所以会使用更多的core，这也就能够说明，为什么当 worker count 在 40 的时候，<font color=red>cpu 利用率</font> 会相差不大的原因
## Gpu 锁

<font color=red size=5>结论</font>：根据如下情况分析，当设置多进程时，cpu 利用率会有提高，但受到 gpu 处理能力的或其他因素的影响，可能提高的幅度有限。

<font color=red>gpu 锁</font> 是由进程决定的，例如，我有两个进程，那么这个 gpu锁 不会相互影响。
1. gpu 锁，当该进程内的线程，想要使用 gpu 时，需要获取 gpu 锁，不同线程之间需要等待锁的释放，才能重新获取锁，导致 cpu 利用率不高。
2. 多进程的情况：根据逻辑推理，多进程之间的 gpu 锁是不同的。所以，当有两个进程时，理想情况是 cpu 的使用率翻倍，但是由于 <font color=red>gpu 处理能力的限制</font> 无法实现 cpu 利用率的大幅度提高。
