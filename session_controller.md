#job #pangen #system
# jobinfo.json
^0b011c
[[jobinfo.json]]
记录了当前job的状态信息，包括session相关信息。
## job信息
- start time： job 开始时间
- first session start time
- job status：
- reason：报错原因
- current session：当前运行的session
- current session id：当前 session 在slurm 中的 jobid 号
- current session status
- session name：该job内的session list
## session 信息
- session name:
- id:
- submit time: session 提交时间
- start time：开始运行的时间
- end time：
- percent complete：进度
- status
- option：是否被保存。（false 表示为被保存）

# log
- checker
- control_prober
- master_session
- prober
- worker_monitor
# scripts
记录了第一个 session 的提交命令
