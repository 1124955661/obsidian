#polygon #EdgeLayer #function 
# 描述
## [[edge layer]] 相关使用
类似 select_polygon_by_relation，额外添加两个参数 with edge 和 without edge，主要描述 polygon 和 edge 之间的关系。当使用这两个参数时，该命令同样需要输入两层layer：layer in和layer reference。最终的结果将从layer in中选出，且layer reference必须是[[edge layer]]。
1. with_edge：将会判断layer in与layer reference 是否满足select edge by relation中的share关系，一旦layer in 中的edge与layer refence中的edge完全共线重叠或部分共线重叠，那么这个该edge所在的polygon就会被选中输出。
2. without_edge：将会判断layer in与layer reference 是否满足select edge by relation中的not share关系。也就是说without edge 是with edge 的反选。
![[Pasted image 20240108110828.png]]
