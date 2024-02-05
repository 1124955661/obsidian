1. ssh  连接用，写一个 脚本去简化用户操作
2. 角色区分，只有管理员和普通用户，管理员可以管理其他用户的job
3. 多 partition提交，在import界面中加入 指定partition的功能。
4. backup 打包，按时间戳去区分命令，再和树彪讨论一下
5. recipe edit：可在 GUI 中编辑当前 Job 的 recipe 文件。弹窗，显示所有的 recipe 文件。
6. sort and filter by column table
	1. project : 同样需要筛选
	2. job name：需要排序或筛选
7. 高级搜索功能，可以通过
8. copy file to，删除该功能。询问 AE 方面，该**功能**的实际需求。
9. 修改资源，worker count，tasks-per-node
10. GUI setting 
	1. ip 和 port 去掉
	2. cpu gpu ratio 可以删除
11. queue 界面 search 直接定位到对应的 job
12. queue ，卡资源，用GPU 限制，需要修改成通过 cpu core 数去限制。同样需要讨论。
13. import 界面，去掉 specified job，会有问题。需要再讨论
14. stauts 加入 waiting，queue 是原来的 submitting
15. 资源显示界面，多分区，修改分区。
16. cksum export 功能，取消在 recipe 里面的 command。在 io_files_cksum.json 中加入一些其他信息。如 topcell。
17. 指定 session，写在 job 表里，显示在 session 列上。