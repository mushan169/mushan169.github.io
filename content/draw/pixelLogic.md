---
date : 2024-03-13
title : 'Pixel Logic的笔记'
tags : ["pixel art"]
summary: '这里是 Pixel Logic的笔记'
---

# Pixel Logic的笔记
## 第一部分 入门：
1. 使用工具：Aseprite

2. sprite： 精灵，是2D游戏中最常见的显示图像的方式，在节点上添加sprite组件，就可以在场景中显示项目资源的图片。

3. sprite放缩的比例：最好是整数倍


4. 对锯齿的处理：不要用更大的像素来包围一行像素
![锯齿处理示例图](/img/pixelLogic/锯齿处理示例图.png)


<center>锯齿处理示例图</center>

>还有一种判断锯齿是否正确的方法，是把线条想象为矢量线条。

1. 黑色内嵌像素画：带有黑色线条的精灵，偶尔也会出现在精灵内部
2. 不同的轮廓线会改变一种精灵的美术风格，任何阶段都会应用线稿

![不同轮廓线风格展示](/img/pixelLogic/不同轮廓线风格展示.png)
<center>不同轮廓线下的风格展示</center>

## 第二部分 抗锯齿
> 抗锯齿的全称为：Anti-Aliased（AA）

抗锯齿的例子：
![](/img/pixelLogic/temmie的例子中来讲抗锯齿.png)

<center>动画师temmie的抗锯齿例子</center>

抗锯齿的技巧：
- 曲线越陡，使用的颜色越少
- 轮廓线颜色深浅的选取：
  - 1. 中间为浅色，两侧为深色。
  - 2. 中间为深色，两侧为浅色。

![](./images/outwards轮廓颜色选取.png)
![](./images/inwards轮廓颜色选取.png)