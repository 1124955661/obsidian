#EdgeLayer #polygon #Edge #function 
# 描述
该命令，可以将输入层的 edge 沿着垂直方向扩展，生成polygon layer 并输出。
```python
pu.edge_expansion(layer,value,extend,direction,option)
```
主要有以下五个参数
1. Layer：支持 [[edge layer]] 和 polygon layer
2. value：设置 expand 的值，可以写成 n * length 这样的表达式
3. extend：可以将 edge 的两个端点沿轴向延长指定的长度，也可以是表达式
4. direction：扩展方向，包含 in（width），out（space），both 方向。
5. option：是一个字典形式，key 是 fill corner，值是 0 或 1，用于控制是否填充expand后生成的polygon的拐角，该值默认为0。当fill corner打开时，extend的值必须为0，并且value不能为n×length的形式。
![[Pasted image 20240108103745.png]]