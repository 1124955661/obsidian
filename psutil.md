#python 
获取系统信息的库

## CPU 信息

```python
>>> import psutil
>>> psutil.cpu_count() # CPU逻辑数量
4
>>> psutil.cpu_count(logical=False) # CPU物理核心
2
# 2说明是双核超线程, 4则是4核非超线程

## 统计 CPU 的用户 / 系统 / 空闲时间
>>> psutil.cpu_times()
scputimes(user=10963.31, nice=0.0, system=5138.67, idle=356102.45)
```