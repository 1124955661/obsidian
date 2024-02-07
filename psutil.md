#python 
获取系统信息的库

## CPU 信息

```python
>>> import psutil
>>> psutil.cpu_count()  CPU逻辑数量
4
>>> psutil.cpu_count(logical=False)  CPU物理核心
2
2说明是双核超线程, 4则是4核非超线程

 统计 CPU 的用户 / 系统 / 空闲时间
>>> psutil.cpu_times()
scputimes(user=10963.31, nice=0.0, system=5138.67, idle=356102.45)

获取 CPU 的使用率
psutil.cpu_percent(interval=1,percpu=True)

```

## 内存信息

```python

psutil.virtual_memory() 获取物理内存信息
svmem(total=8589934592, available=2866520064, percent=66.6, used=7201386496, free=216178688, active=3342192640, inactive=2650341376, wired=1208852480)

psutil.swap_memory() 获取交换内存信息
sswap(total=1073741824, used=150732800, free=923009024, percent=14.0, sin=10705981440, sout=40353792)

```

## 磁盘信息
```python
>>> psutil.disk_partitions()  磁盘分区信息
[sdiskpart(device='/dev/disk1', mountpoint='/', fstype='hfs', opts='rw,local,rootfs,dovolfs,journaled,multilabel')]

>>> psutil.disk_usage('/')  磁盘使用情况
sdiskusage(total=998982549504, used=390880133120, free=607840272384, percent=39.1)

>>> psutil.disk_io_counters()  磁盘IO
sdiskio(read_count=988513, write_count=274457, read_bytes=14856830464, write_bytes=17509420032, read_time=2228966, write_time=1618405)
```

## 网络信息

```python
>>> psutil.net_io_counters() # 获取网络读写字节／包的个数
snetio(bytes_sent=3885744870, bytes_recv=10357676702, packets_sent=10613069, packets_recv=10423357, errin=0, errout=0, dropin=0, dropout=0)
>>> psutil.net_if_addrs() # 获取网络接口信息
{
  'lo0': [snic(family=<AddressFamily.AF_INET: 2>, address='127.0.0.1', netmask='255.0.0.0'), ...],
  'en1': [snic(family=<AddressFamily.AF_INET: 2>, address='10.0.1.80', netmask='255.255.255.0'), ...],
  'en0': [...],
  'en2': [...],
  'bridge0': [...]
}
>>> psutil.net_if_stats() # 获取网络接口状态
{
  'lo0': snicstats(isup=True, duplex=<NicDuplex.NIC_DUPLEX_UNKNOWN: 0>, speed=0, mtu=16384),
  'en0': snicstats(isup=True, duplex=<NicDuplex.NIC_DUPLEX_UNKNOWN: 0>, speed=0, mtu=1500),
  'en1': snicstats(...),
  'en2': snicstats(...),
  'bridge0': snicstats(...)
}
```