#edge
# Define
首先，block edge必须来自于执行[[dimensional check]]的layer1或者layer2，它可以是一段完整的edge，也可以是被打断后的edge segment。也就是说如果来自不同layer的edge存在相交的情况，在交点处则会打断edge。

其次，Block edge的一端必须与那些满足selection rule的原始pair edge的端点相连。

如果block edge能够把pair edge生成的region完全切断分成多个area，那么这一对pair edge的结果则是无效的，在标准结果下该对pair edge不会输出。

当metric是Euclidean和square 时，constraint中的min value必须写成0，即下限必须是>0或>=0。否则block edge的限制会失效。而在opposite metric中，block edge不会对pair edge的结果有所限制。

以下面三张图为例，左图中红色的一对边组成了pair edge，layer1中那条竖直方向的长边与红色边首尾相连，另一方面，由于该竖直边与来自layer2的水平边相交，所以在交点处产生break点，实际的block edge只是黑色的那段edge segment。该段edge segment并没有把pair edge的region完全切断为两部分，所以该段pair edge及其region最终是可以输出的。

在中间这个图中，绿色的region能够完全被黑色的竖直block edge切断，所以该region及其对应的pair edge是无效的，在标准结果下该对pair edge不会输出。

在第三图中，由于constraint的下限被设置成一个非零的正数，所以尽管在该pair edge的region内存在一条block edge能够完全把region分为两部分，block edge仍会被认作是无效的。
![[Pasted image 20240102104108.png]]
