---
title: “陆空赛跑”
date: 2022-12-20
excerpt_separator: "<!--more-->"
categories: 
  - SVG制作
tags:
  - svg
---

惊现城市里竟有一辆飞机与火车在赛跑，这到底是怎么回事？

<!--more-->

#### 静态飞机与货车
以下是我在[ **Font Awesome** ](https://fontawesome.com/)上找到的飞机以及货车素材。

<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" width="10%"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M482.3 192c34.2 0 93.7 29 93.7 64c0 36-59.5 64-93.7 64l-116.6 0L265.2 495.9c-5.7 10-16.3 16.1-27.8 16.1l-56.2 0c-10.6 0-18.3-10.2-15.4-20.4l49-171.6L112 320 68.8 377.6c-3 4-7.8 6.4-12.8 6.4l-42 0c-7.8 0-14-6.3-14-14c0-1.3 .2-2.6 .5-3.9L32 256 .5 145.9c-.4-1.3-.5-2.6-.5-3.9c0-7.8 6.3-14 14-14l42 0c5 0 9.8 2.4 12.8 6.4L112 192l102.9 0-49-171.6C162.9 10.2 170.6 0 181.2 0l56.2 0c11.5 0 22.1 6.2 27.8 16.1L365.7 192l116.6 0z"/></svg>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512" width="10%"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M112 0C85.5 0 64 21.5 64 48V96H16c-8.8 0-16 7.2-16 16s7.2 16 16 16H64 272c8.8 0 16 7.2 16 16s-7.2 16-16 16H64 48c-8.8 0-16 7.2-16 16s7.2 16 16 16H64 240c8.8 0 16 7.2 16 16s-7.2 16-16 16H64 16c-8.8 0-16 7.2-16 16s7.2 16 16 16H64 208c8.8 0 16 7.2 16 16s-7.2 16-16 16H64V416c0 53 43 96 96 96s96-43 96-96H384c0 53 43 96 96 96s96-43 96-96h32c17.7 0 32-14.3 32-32s-14.3-32-32-32V288 256 237.3c0-17-6.7-33.3-18.7-45.3L512 114.7c-12-12-28.3-18.7-45.3-18.7H416V48c0-26.5-21.5-48-48-48H112zM544 237.3V256H416V160h50.7L544 237.3zM160 464c-26.5 0-48-21.5-48-48s21.5-48 48-48s48 21.5 48 48s-21.5 48-48 48zm368-48c0 26.5-21.5 48-48 48s-48-21.5-48-48s21.5-48 48-48s48 21.5 48 48z"/></svg>
			
#### 飞机与货车赛跑赛了一整天
通过添加代码，实现了css背景渐变的动画，运用svg的移动这种动画，来实现飞机与货车的赛跑。

![](/assets/images/SVG制作/2022-12-20-world_code.png)

接下来呈现出画面：
<style>
.box{
	width: 1500px;
	height: 780px;
	background: #87CEEB;
	animation:myfirst 15s;
	-webkit-animation:myfirst 10s; /* Safari and Chrome */
	animation-iteration-count: infinite;
}

@keyframes myfirst
{
	from { background-image: linear-gradient(#7ce6dd, #ffffff);}
	to { background-image: linear-gradient(#ffe96a, #ff5f15);}
}

@-webkit-keyframes myfirst /* Safari and Chrome */
{
	from { background-image: linear-gradient(#7ce6dd, #ffffff);}
	to { background-image: linear-gradient(#ffe96a, #ff5f15);}
}

.plane{
	width: 300px;
	top: 0px;
	animation: second 3s infinite linear;
}

@keyframes second{
	to{
		transform: translateX(1500px);
	}
}

.track{
	width: 200px;
	/*position: absolute;*/
	bottom: 0px;
	animation: third 10s infinite ease;
}

@keyframes third{
	from{
		left: 0px;
	}
	to{
		transform: translateX(1500px);
	}
}

</style>

<div class="box">

			
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 576 512" class="plane"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M482.3 192c34.2 0 93.7 29 93.7 64c0 36-59.5 64-93.7 64l-116.6 0L265.2 495.9c-5.7 10-16.3 16.1-27.8 16.1l-56.2 0c-10.6 0-18.3-10.2-15.4-20.4l49-171.6L112 320 68.8 377.6c-3 4-7.8 6.4-12.8 6.4l-42 0c-7.8 0-14-6.3-14-14c0-1.3 .2-2.6 .5-3.9L32 256 .5 145.9c-.4-1.3-.5-2.6-.5-3.9c0-7.8 6.3-14 14-14l42 0c5 0 9.8 2.4 12.8 6.4L112 192l102.9 0-49-171.6C162.9 10.2 170.6 0 181.2 0l56.2 0c11.5 0 22.1 6.2 27.8 16.1L365.7 192l116.6 0z"/></svg>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 640 512" class="track"><!--! Font Awesome Pro 6.2.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M112 0C85.5 0 64 21.5 64 48V96H16c-8.8 0-16 7.2-16 16s7.2 16 16 16H64 272c8.8 0 16 7.2 16 16s-7.2 16-16 16H64 48c-8.8 0-16 7.2-16 16s7.2 16 16 16H64 240c8.8 0 16 7.2 16 16s-7.2 16-16 16H64 16c-8.8 0-16 7.2-16 16s7.2 16 16 16H64 208c8.8 0 16 7.2 16 16s-7.2 16-16 16H64V416c0 53 43 96 96 96s96-43 96-96H384c0 53 43 96 96 96s96-43 96-96h32c17.7 0 32-14.3 32-32s-14.3-32-32-32V288 256 237.3c0-17-6.7-33.3-18.7-45.3L512 114.7c-12-12-28.3-18.7-45.3-18.7H416V48c0-26.5-21.5-48-48-48H112zM544 237.3V256H416V160h50.7L544 237.3zM160 464c-26.5 0-48-21.5-48-48s21.5-48 48-48s48 21.5 48 48s-21.5 48-48 48zm368-48c0 26.5-21.5 48-48 48s-48-21.5-48-48s21.5-48 48-48s48 21.5 48 48z"/></svg>
			
			
</div>