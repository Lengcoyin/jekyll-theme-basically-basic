---
layout: page
title: 玩转“border-radius”
date: 2022-12-25
excerpt_separator: "<!--more-->"
categories:
     - 平面设计
---

使用CSS中的border-radius属性，可以给任何元素制作圆角，快来试试吧！

<!--more-->

#### border-radius代码的一般写法

【border-radius: 110px;】
这是一般写法，这样矩形的四角就会自动变为相应数值的圆角。

因为我们只输入了一个数值，所以所有角都会被四舍五入，若要固定值可以使用 px，百分比(%)就使用 rem, em这些单位。

接下来我们来观察一下「border-radius: 110px」与「border-radius: 30%」的矩形的区别：
![](assets/images/pmsj/yuanjiao_compare.png)
由此我们可以看出，两者的圆角是不对称的，「border-radius: 110px」的图形的圆角会更圆润些。

#### border-radius用4个值的样式

当设置多个 border-radius 数值时，从左上角开始顺时针设置，还可以使用百分比单位，甚至可以与固定值混合使用。
![](assets/images/pmsj/yuanjiao_four.png)

#### border-radius还可以用8个值的样式

Border-radius 最多可以使用8个数值，但是注意，需要作用斜杠「 / 」来分隔4个值！！！
如果在斜杠前后设置一个值，则斜杠前面的值设置水平半径，斜杠后面的值设置垂直半径。如果没有斜杠，则该值将两个半径设置为相等。

为了更好的理解：
![](assets/images/pmsj/yuanjiao_eight.png)
其实也就是四个重叠的椭圆，构成最终的形状，像是4个立体图形最后构成平面图。这也需要我们更加清晰理解这项属性的规范书写。


更多详情:
[W3C](https://www.w3.org/TR/css-backgrounds-3/#border-radius)