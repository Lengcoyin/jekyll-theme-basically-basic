---
layout: page
title: 页面的条理性还是得看响应式网格视图
date: 2022-12-25
excerpt_separator: "<!--more-->"
categories:
     - 平面设计
---

很多网页都是基于网格设计的，这说明网页是按列来布局的。
使用网格视图有助于我们设计网页。这让我们向网页添加元素变的更简单。让我们一起来研究一下吧！

<!--more-->

#### 响应式网格视图

首先确保所有的 HTML 元素都有 box-sizing 属性且设置为 border-box。如下图
![](assets/images/pmsj/2022-12-25-net_code.png)
再对宽度、边距等参数进行调整后可以得出像这样的设计：
![](assets/images/pmsj/2022-12-25-netu.png)

#### 美化以及更好地控制响应式网页

通过计算，我们得知12列的网格系统可以更好的控制响应式网页,这样在浏览器窗口大小调整时会自动伸缩。
计算出每列的百分比:100%/12列=8.33%。在每列中指定 class， class="col-" 用于定义每列有几个span。
![](assets/images/pmsj/2022-12-25-neta_code.png)

通过加入一些样式再进行美化这个网格视图以及上方12列的网格系统控制得出：
![](assets/images/pmsj/2022-12-25-netb.png)
