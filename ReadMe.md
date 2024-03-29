#旅行规划辅助决策系统

基本理论：《有序构建》

流程模型理论：
理论基础，所有的计算机解决的问题都始于模拟，比如整个冯诺依曼系统就是对现实的一个最大的模拟，CPU创造了时间，内存和硬盘创造了存储（空间和变化）， 而在这个基础架构之上运行的东西是一个个过程或者流程。这个和现实世界的状况基本类似。因而，对于旅行规划的辅助决策系统，我们要做的是就是建立整个旅行规划的流程模型。

流程模型最主要的组成部分：

1. 关键概念
2. 关系

任何一个流程都是这两部分组成，只不过是数量的问题。而在编程的时候，我们能够处理的是三维空间结构，我们正式要通过三维空间结构模拟出四维的时序结构。因为我们无法在静止的三维空间中，真正的理解四维时序结构的样子。因而在模拟的时候我们会采取描述的方式来解决。


关键的策略：

1. 模拟
2. 描述

然而又一个问题是，我们很难穷举在整个旅行规划流程中，所有的概念和关系(这实际到多层级概念簇和关系之间叠加，夸概念和关系的抽象切割等问题)，因为，我们要构建的是一套能够自我生成概念和关系的系统。

```
结果<---施加约束---流程<-------概念和关系<--输出--概念和关系生成系统<------输入---旅行信息
```


前期最核心的东西就是概念和关系生成的这个系统的建设。

但是他的理论基础是什么？如何自动的从数据中生成概念和关系，从而找到流程，目前那些学科的知识或者理论能够帮助到？知识边际所及范围之内能够看到的是，机器学习理论。

####基础系统之一
***时序流程抽取***

将旅行的数据，整理成具有时序关系的流程数据。然后在这些流程数据之上使用聚类算法，抽取概念和关系。