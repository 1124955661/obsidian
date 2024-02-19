#job #JobManager 
## 问题
1. 当 rerun 的时候，由于第一次运行的session 导致 判断条件 变化，
	1. 第一次运行 job，走的是 if 路线，但是某个 session 导致判断条件变化了。
	2. 第二次指定运行 if 路线中的 session 时，但是由于判断条件变化，将执行 else 路线
2. 当某条路线中有多个 session 时，如 if 路线中 有 session A1，A2，A3
	1. 当指定 A1 rerun 时，A2，A3 将会被从option session 记录中删除
	2. 指定 A3，对 A1，A2 无影响
3. 当 if-else 的 session 位于 job 的最后时，同理如存在session B1，B2，B3 
	1. 无论指定B1，B2，B3 中的哪个 session，都会将其之后的 session 全部运行完。