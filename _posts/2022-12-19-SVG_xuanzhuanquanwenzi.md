---
title: 一直运转的是我们坚信的信仰
date: 2022-12-19
excerpt_separator: "<!--more-->"
categories: 
  - SVG制作
tags:
  - svg
---

如何在自己的页面显示一个svg动画呢？

<!--more-->

### 运转的文字圈
以下是我在[ **ANIMPEN码笔网** ](http://animpen.com/search/pens/?q=svg)上找到的一个旋转文字，原动画是这样。

<style>@keyframes rotate {
	to {
		transform: rotate(360deg);
	}
}

svg {
	width: 35vw;
	height: 35vw;
	animation: rotate linear 20s infinite;
}

svg text {
	font-size: 30px;
	fill: white;
}

body {
	height: 100vh;
	margin: 0;
	background: #161616;
	display: flex;
	justify-content: center;
	align-items: center;
	font-family: "Roboto Condensed", sans-serif;
	text-transform: uppercase;
}
</style>


<svg viewBox="-126 -126 252 252" xmlns="http://www.w3.org/2000/svg">
	<path id="path" d="M-125 0a125 125 0 10250 0 125 125 0 10-250 0" fill="none" />
	<text y="40">
		<textPath href="#path" startOffset="20"> We have only the dream To see what you wanted to be
		</textPath>
	</text>
</svg>


### 运转着背景变色的文字圈

接着我增加了一段改变背景色的动画代码样式：

![](/assets/images/SVG制作/circle_code.png)

于是一个根据有意义的粉蓝背景色进行变色的运转文字圈就完成啦！
一直运转的文字是我目前最向往的希望，而这也是我坚信的永远不会改变的信仰。

<style>
@keyframes rotate {
	to {
		transform: rotate(360deg);
	}
}


svg {
	width: 35vw;
	height: 35vw;
	border-radius: 40px;
	animation: rotate linear 15s infinite;

}


svg text {
	font-size: 30px;
	fill: white;
}

body {
	/*height: 100vh;*/
	margin: 0;
	background-color: skyblue;
	height: 900px;
	background-image: linear-gradient(skyblue,pink);
	display: flex;
	justify-content: center;
	align-items: center;
	font-family: "arial black", sans-serif;
	text-shadow: 5px 5px 5px gainsboro;
	text-transform: uppercase;
}

@keyframes rotate
{
	to{
		transform: rotate(360deg);
	}
    0%   {background: skyblue;}
    25%  {background: lightblue;}
    50%  {background: pink;}
    75%  {background: #FFC0CB; }
    100% {background: skyblue;}
}
 
@-webkit-keyframes rotate /* Safari 与 Chrome */
{
	to{
		transform: rotate(360deg);
	}
    0%   {background: skyblue;}
    25%  {background: lightblue;}
    50%  {background: pink;}
    75%  {background: #FFC0CB;}
    100% {background: skyblue;}
}

</style>


<svg viewBox="-126 -126 252 252" xmlns="http://www.w3.org/2000/svg">
			<path id="path" d="M-125 0a125 125 0 10250 0 125 125 0 10-250 0" fill="none" />
			<text y="40">
				<textPath href="#path" startOffset="20"> SEVENTEEN AND CARAT FOREVER TOGETHER
				</textPath>
			</text>
		</svg>



