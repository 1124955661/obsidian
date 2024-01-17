#问题 #system
# 情形

worker 起来了，有log，log中的 上一个 **read command end** 到下一个 **read command begin** 之间的间隔很长
# 解决步骤

注释掉 merge 命令
