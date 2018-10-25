# Deep-learning-CNN-demo
对经典卷积神经网络的实现练习
主要来自于Tensorflow实战（黄文坚）
附上经典的神经网络论文


## LeNet
LeNet主要提出了CNN的概念，非常划时代，论文主体分析了Traditional pattern recognition的劣势和卷积神经网络的三大核心思想
### 传统的图像识别劣势
* have no built-in invariance
* 忽略了输入的拓扑结构
### CNN三大核心思想
* 局部感受野：基于图像局部相关的原理，保留了图像局部结构，同时减少了网络的权值（每个神经元不必感受整副图像，只需要感受局部）
* 权值共享： 基于图像局部的原理，同时减少网络的权值参数
(局部感受野类似于图像的卷积操作，能够提取局部特征，
而图像局部特征检测器也可以用于整个图像，这样就可以提取整幅图像的特征，基于这个特征，
我们可以将局部感受野位于不同位置的神经元设置为相同的权值，这些输出CNN中的一个特征图)
* 下采样： 下采样可以降低特征位置的精度，使得对平移和形变更加鲁棒
