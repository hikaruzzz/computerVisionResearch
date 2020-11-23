# 计算机视觉 学习指导

## 目录：
1.	研究方向介绍
2.	学习思路
3.	最后


## 1. 研究方向介绍
计算机视觉领域按照任务可以分成几大类：分类[classification](https://www.paperswithcode.com/area/computer-vision/image-classification)、分割（语意分割[semantic segmentation](https://www.paperswithcode.com/area/computer-vision/semantic-segmentation)、实例分割[instance segmentation](https://www.paperswithcode.com/task/instance-segmentation)）、目标检测[object detection](https://www.paperswithcode.com/area/computer-vision/object-detection)、生成[generation](https://www.paperswithcode.com/area/computer-vision/image-generation)、姿态估计[post estimation](https://www.paperswithcode.com/area/computer-vision/pose-estimation)、弱监督([few-shot,one-shot](https://www.paperswithcode.com/area/computer-vision/few-shot-learning))等等。其每个大类中也有多个细分类，具体可以参考这个链接：
* https://www.paperswithcode.com/area/computer-vision 

以上这些类别都基于图像、视频等2D数据，最近几年出现了很多基于3D数据（比如点云）的神经网络模型研究，和图像一样，他们也都分别面向分类、分割、生成等任务。下面归类了一些由数据集驱动的研究方向，可以尝试在这些数据集的benchmark中找个比较领先的模型代码入手学习。

#### 数据集驱动的一些研究方向以及有代表性的数据集：
| 数据集类型 |任务   | 数据集 |
|:-:|:-:|:-:| 
| 图像| 分类任务 | [imageNet](https://www.paperswithcode.com/sota/image-classification-on-imagenet) | 
|图像| 目标检测|[COCO](https://www.paperswithcode.com/sota/object-detection-on-coco-minival) | 
|图像|分割任务|[Cityscapes](https://www.paperswithcode.com/sota/semantic-segmentation-on-cityscapes-val) |
| 点云| 分类任务|[ModelNet](https://www.paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40) |
|点云|分割任务| [S3DIS](https://www.paperswithcode.com/sota/semantic-segmentation-on-s3dis)、[ScanNet](https://www.paperswithcode.com/sota/semantic-segmentation-on-scannet) |


## 2. 学习思路
从一个研究领域入手，可以找这个方向的一些综述文献或者博客看看，比如下面这些：
* 图像语义分割:  
https://arxiv.org/pdf/1704.06857.pdf 

* 图像目标检测:  
https://www.jiqizhixin.com/articles/2018-04-27?from=synced&keyword=%E7%9B%AE%E6%A0%87%E6%A3%80%E6%B5%8B%E7%AE%97%E6%B3%95 

或者在一些高引用的论文的relation work章节中了解一些同类研究工作，了解当前的研究现状，了解哪些方法有参考价值。  
#### 一些高引用的论文： 
* 点云语义分割:  
https://arxiv.org/pdf/1904.08889v2.pdf 
* 点云分类:  
https://arxiv.org/pdf/1612.00593v2.pdf 

## 3. 最后
多看论文，聚焦到某个细分领域，看看这个细分领域中的研究工作都是围绕些什么问题做研究的，这些就是 “该领域的痛点“，然后分析大家提出的想法是怎么解决这些问题的，也可以多学习其他领域的文献，想想看能不能从其他领域借鉴一些解决办法。

寻找一些经典模型 (比如高引用论文的模型) 作为baseline，在这些baseline上面去做小的创新性改动，实现新想法，验证效果，同一个数据集中对比baseline和新方法的效果，当改进方法的创新性和实验效果到了一定程度，就可以考虑发表论文了。
