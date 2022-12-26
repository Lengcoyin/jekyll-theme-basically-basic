---
layout: page
title: “你站这我站哪”之定位布局
date: 2022-12-26
excerpt_separator: "<!--more-->"
categories:
     - 学习笔记
---

不知道有没有友友和我一样，对定位布局的运用不太清楚呢？跟着我一起梳理知识吧。

<!--more-->

#### 三种定位布局
![](assets/images/studynotes/position_three.jpg)

对于这三种定位我的理解是：
1.fixed是相对于整个网页浏览器去定位，定的点是以浏览器为基准的。
2.relative是相对于元素自己本身上一次（原本）的位置来进行定位，是以微调为主。
3.absolute是三者当中找起来最麻烦的一个，他是根据其最近的已定位的父级原点(relative对象)去定,如果父级没有定位，会找父级的父级原点的定位。

还有一种固定定位的例子，我们也需要理解清楚
![](assets/images/studynotes/position_guding.png)

- 其中注意，设置偏移量时，left和top的优先级高于right和bottom。
- 补充说明，[Margin: 0 auto;] 可以让元素居中
- 添加[overflow：hidden/auto/scroll] 的属性可以使长段文字加入侧边的滚动进度条。
- 添加[:hover] 鼠标移入或停留。

补充说明部分可以使我们的网页与用户更具有交互性，同时也是使页面更美观的几种方法。



* 其实定义最多也只是文字，更重要的还是需要我们亲手去实践一下，这样才能知道我们想要的元素位置到底应该放在哪里。

这是对定位布局所进行的练习
![](assets/images/studynotes/position_lianxi.png)

同时也对其进行了响应式设计
![](assets/images/studynotes/position_lianxi2.png)




更多请参考:[css定位](https://www.runoob.com/css/css-positioning.html)
