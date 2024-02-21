---
title: jmmaster log
date created: 星期三, 一月 3日 2024, 9:41:14 上午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

# 提交相关
如图所示，当一个job要提交时，可以查看这部分log信息，关键字 ==remoteCommand==，这里包含被提交的job的关键信息。该部分信息为请求部分。

当请求部分信息结束后，会检查==资源==相关信息和当前**队列**的状态。
![[Pasted image 20240103094154.png]]
如下图所示，会先执行checkEnoughResource 这个函数，检查当前集群内的资源是否充足。

![[Pasted image 20240103095856.png]]