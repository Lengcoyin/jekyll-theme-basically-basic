---
layout: page
title: 媒体查询与弹性布局
date: 2022-12-26
excerpt_separator: "<!--more-->"
categories:
     - 学习笔记
---

什么是媒体查询？弹性布局我们又能运用在哪里呢？他对我们的用处大吗？让我们一起来看一下吧。

<!--more-->

#### 媒体查询的定义及使用
使用 @media 查询，你可以针对不同的媒体类型定义不同的样式。
@media 可以针对不同的屏幕尺寸设置不同的样式，特别是如果你需要设置设计响应式的页面，@media 是非常有用的。
当你重置浏览器大小的过程中，页面也会根据浏览器的宽度和高度重新渲染页面。

媒体查询的写法：
![](assets/images/studynotes/media_write.png)

以下是课堂上举的例子，将两行代码变换成文字语言叙述明白：
![](assets/images/studynotes/media_screen.jpg)

- 注意，媒体查询中所出现的关键字：
- and：可以将多个媒体特性连接一起
- not：排除某个媒体类型
- only：指定某个特定的媒体类型

如：@import url (“tiny.css”) screen and (min-width:200px) and (max-width:360px);使用最大宽度（max-width) 和最小宽度（min-width）设定了范围。因此，tiny.css只在设备视口介于200px和360px之间时才会被应用。
#### viewport
这里再加上viewport的知识点
![](assets/images/studynotes/media_viewpoint.jpg)
- content=“ maximum-scale=2.0” 允许用户最大将页面放大到设备宽度的两倍- content=“ minimum-scale=0.5” 允许用户最小将页面缩小到设备宽度的一半- user-scalable=no   禁止用户缩放- user-scalable=yes  允许用户缩放

##### 弹性布局
为什么将媒体查询与弹性布局放在一起讲呢？
因为他们所呈现出来的效果目的是相同的道理。

flex布局则是一种新的布局方案，通过为修改父div的display属性，让父元素成为一个flex容器，从而可以自由的操作容器中子元素(项目)的排列方式。
它可以自动调整，计算元素在空间中的大小，从而进行合理的布局。
- 这样恰当运用的弹性布局对用户十分友好，页面中的所有元素可以随着用户的偏好缩放，这也可以使用户获得一个很好的体验感以及观感。

flexbox的属性：
![](assets/images/studynotes/flex_a.jpg)
![](assets/images/studynotes/flex_b.jpg)


媒体查询与弹性布局我认为对于网页来说是一个重要的性能，他决定着这个网页在不同的媒体或是不同大小的观看屏幕上
可以有着最优的观感及交互体验感。同时也是让网页在任何媒体都能保持最优美的，不被遮挡或是缺失一部分应用能力。
这样能够让用户获得相应的合适的互动才是最重要的，所以赶紧动手练起来吧！