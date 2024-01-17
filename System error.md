#bug #system #job #run 
# [[boost::filesystem::remove: Directory not empty]]
## 现象
1. job 开始running之后，快速转变状态至 ==done==， 然后job 无法运行。

## 操作
1. 使用[[job manager]] 先将 job 复制到工作路径下
2. 直接在 terminal 中手动提交该job。