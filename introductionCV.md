计算机视觉 研究入门指导

目录：
1.	研究方向介绍
2.	各模型的开源代码
3.	研究思路

1.	研究方向介绍
计算机视觉领域按照任务可以分成几类：分类、分割（语意分割、实例分割）、目标检测、生成、姿态估计等。其每个大类中也有多个细分类，具体可以参考这个链接：
https://www.paperswithcode.com/area/computer-vision 

以上这些类别都基于图像、视频等2D数据，最近几年才有了很多基于3D数据（比如点云）的神经网络模型研究，和图像一样，他们也都分别面向分类、分割、生成等任务。

数据集驱动的一些研究方向以及有代表性的数据集：
图像分类任务：imageNet		|	分割任务：Cityscapes	|	目标检测：COCO
点云分类任务：ModelNet40	|	分割任务：S3DIS、ScanNet

2.	各模型的开源代码
对于开源代码，可以在那些有代表性的数据集benchmark中找领先模型的代码，比如：图像语义分割任务
https://www.paperswithcode.com/sota/semantic-segmentation-on-cityscapes

点云语义分割任务
https://www.paperswithcode.com/sota/semantic-segmentation-on-scannet 

3.	研究思路
从一个研究领域入手，可以找这个方向的一些综述文献或者博客看看，比如下面这些：
https://arxiv.org/pdf/1704.06857.pdf （图像语义分割）

https://www.jiqizhixin.com/articles/2018-04-27?from=synced&keyword=%E7%9B%AE%E6%A0%87%E6%A3%80%E6%B5%8B%E7%AE%97%E6%B3%95 （图像目标检测）

或者在一些高引用的论文中的relation work中了解一些同类研究工作，比如这些论文：
https://arxiv.org/pdf/1904.08889v2.pdf (点云分割)

https://arxiv.org/pdf/1612.00593v2.pdf (点云分类)

多看论文，聚焦到某个细分领域，看看这个细分领域中的研究工作都是围绕些什么问题做研究的，这些就是“领域痛点“，然后分析大家是怎么解决的，多看文献，想想看能不能从其他领域借鉴一些解决办法。

寻找一些经典模型(比如高引用论文的模型)作为baseline，在这些baseline上面去做小的创新性改动，实现idea，验证效果，同一个数据集对比baseline和新方法的效果，当改进方法的创新性到了一定程度，就可以考虑发表论文了。
