---
layout: page
title: 标签的“名字”
date: 2022-12-27
excerpt_separator: "<!--more-->"
categories:
     - 学习笔记
---

在学习html之前，我们需要打好基础，了解标签的种类还有书写规范哦。

<!--more-->

#### 常见标签
- title标签
写法：< title >< /title >双标签语义：网页标题权重最大- h标签H1~h6双标签语义：标题默认样式：font-size、font-weight、margin权重：h1>h2>h3>h4>h5>，页面中h1最好不要超过1个，h2不要超过12个，h3之后随便- div标签双标签语义：无意义默认样式：无
#### 新语义标签
- 语义化标签：HTML5引入了新的HTML元素，通过使用这些元素，开发者可以更细致的描述文档结构，让文档更加易读，搜索引擎也能更好的理解页面中各部分间的关系，我们也可以搜索到更快、更准确的信息。例如div标签，我们用id命名网页的基本结构，这时搜索引擎无法识别id的命名，对他而言这只是一块块区域。
所以便有了
- nav                语义：导航
- footer        语义：文档或页面的脚部，通常包含版权信息、联系方式、友情链接- aside           语义：侧边栏、附属信息
- article    语义：定义一个独立内容区块（如文章、视频文件）
- section    语义：定义一个区域，如文章的章节等

更多请参考：[HTML5所有标签](https://www.w3.org/TR/html5/semantics.html#semantics)
* HTML5新语义标签更注重于内容而不是形式,更加语义化，高度描述性，更加直观，增加了代码的可读性,同时浏览器更容易解析，搜索引擎更容易抓取文档内容。

![](assets/images/studynotes/biaoqian1.jpg)
![](assets/images/studynotes/biaoqian2.jpg)


#### 块标签与内联标签
- 块标签的特点：
1.总是在新行上开始
2.高度，行高以及顶和底边距都可控制
3.宽度缺省是它的容器的100%，除非设定一个宽度
4.div,p,h1,form,ul和li是块元素的例子

- 内联标签的特点：
1.和其他元素都在一行上
2.高，行高及顶和底边距不可改变
3.宽度就是他的文字或图片的宽度，不可改变
4.span,a,label,input,img,strong,em是inline元素的例子
5.内联元素只能容纳文本或其他内联元素


注意：
1. 块级元素可以包含内联元素或某些块级元素，但内联元素不能包含块级元素，他只能包含其他内联元素。
2. 块级元素不能放在p里面。
3. 特殊的块级元素只能包含内联元素，不能包含块级元素。如h1,h2,h3,p,dt
4. li内可以包含div
5. 块级元素与块级元素并列、内联元素与内联元素并列。

#### a标签和img标签
![](assets/images/studynotes/biaoqian_img.png)
a href="需要链接的网页地址" target="打开网页的方式"></
img src="图片的路径地址" alt="图片说明">


更多请看：[更多](https://www.w3school.com.cn/html/html5_semantic_elements.asp)

