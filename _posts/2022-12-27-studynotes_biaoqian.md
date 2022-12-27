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
写法：< title >< /title >双标签语义：网页标题权重最大- h标签H1~h6写法：<h1></h1><h2></h2><h3></h3><h4></h4><h5></h5><h6></h6>双标签语义：标题默认样式：font-size、font-weight、margin权重：h1>h2>h3>h4>h5>，页面中h1最好不要超过1个，h2不要超过12个，h3之后随便- div标签
写法：<div></div>双标签语义：无意义默认样式：无
#### 新语义标签
- 语义化标签：HTML5引入了新的HTML元素，通过使用这些元素，开发者可以更细致的描述文档结构，让文档更加易读，搜索引擎也能更好的理解页面中各部分间的关系，我们也可以搜索到更快、更准确的信息。例如<div>标签，我们用id命名网页的基本结构，这时搜索引擎无法识别id的命名，对他而言这只是一块块区域。
所以便有了
- <nav></nav>                语义：导航
- <footer></footer>        语义：文档或页面的脚部，通常包含版权信息、联系方式、友情链接- <aside></aside>           语义：侧边栏、附属信息
- <article></article>    语义：定义一个独立内容区块（如文章、视频文件）
- <section></section>    语义：定义一个区域，如文章的章节等

更多请参考：[HTML5所有标签](https://www.w3.org/TR/html5/semantics.html#semantics)
* HTML5新语义标签更注重于内容而不是形式,更加语义化，高度描述性，更加直观，增加了代码的可读性,同时浏览器更容易解析，搜索引擎更容易抓取文档内容。

![id](assets/images/studynotes/biaoqian1.jpg)
![ud](assets/images/studynotes/biaoqian2.jpg)


#### 块标签与内联标签
- 块标签的特点：
![块标签](assets/images/studynotes/biaoqian_block.png)

- 内联标签的特点：
![内联标签](assets/images/studynotes/biaoqian_inline.png)


注意：
1.块级元素可以包含内联元素或某些块级元素，但内联元素不能包含块级元素，他只能包含其他内联元素。
2.块级元素不能放在p里面。
3.特殊的块级元素只能包含内联元素，不能包含块级元素。如h1,h2,h3,p,dt
4.li内可以包含div
5.块级元素与块级元素并列、内联元素与内联元素并列。

#### a标签和img标签
![a标签与img标签](assets/images/studynotes/biaoqian_img.png)



更多请看：[更多](https://www.w3school.com.cn/html/html5_semantic_elements.asp)

