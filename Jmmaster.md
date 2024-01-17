---
aliases:
---

#tool #server
该工具是，[[job manager]] 的后台服务端，所有和 slurm或是job之间的交互都需要通过这个 服务端处理。

```xml
# jmmaster.conf

  1 <?xml version="1.0" encoding="UTF-8" standalone="yes"?>
  2 <root>
  3     <jmmaster>
  4         <port>8105</port>
  5         <threadnums>5</threadnums>
  6         <publicpath>/home/temp/jobmanager</publicpath>
  7     </jmmaster>
  8 </root>
```

# [[jmmaster log]]
通过log，去对异常现象进行debug。