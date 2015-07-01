动画
====

CSS3，我们可以创建动画，它可以取代许多网页动画图像，Flash 动画，和 Javascripts。

## CSS3 @keyframes 规则
要创建CSS3动画，你将不得不了解`@keyframes`规则。

`@keyframes`规则是用来创建动画。 `@keyframes`规则内指定一个 CSS样式和动画将逐步从目前的样式更改为新的样式。

**注意：**Internet Explorer 10、Firefox 以及 Opera 支持 `@keyframes` 规则和 animation 属性。
Chrome 和 Safari 需要前缀 -webkit-。

## CSS3 动画
当在`@keyframe`创建动画，把它绑定到一个选择器，否则动画不会有任何效果。

指定至少这两个 CSS3 的动画属性绑定向一个选择器：

* 规定动画的名称
* 规定动画的时长

例子：

    #animated_div {
        animation: animated_div 5s infinite;
        -moz-animation: animated_div 5s infinite;
        -webkit-animation: animated_div 5s infinite;
    }

## CSS3动画是什么？

* 动画是使元素从一种样式逐渐变化为另一种样式的效果。
* 您可以改变任意多的样式任意多的次数。
* 请用百分比来规定变化发生的时间，或用关键词 "from" 和 "to"，等同于 0% 和 100%。
* 0% 是动画的开始，100% 是动画的完成。
* 为了得到最佳的浏览器支持，您应该始终定义 0% 和 100% 选择器。

例子：

	@keyframes animated_div {
		0% {
		    left: 0px;
		}
		20% {
		    left: 50px;
		    background-color: green;
		}
		40% {
		    left: 140px;
		    background-color: red;
		}
		60% {
		    left: 280px;
		    background-color: yellow;
		}
		80% {
		    left: 425px;
		    background-color: blue;
		}
		100% {
		    left: 0px;
		    background-color: pink;
		}
	}

## 常用属性

<table class="reference"> <tbody><tr> <th style="width:30%;">属性</th> <th>描述</th> <th style="width:5%;">CSS</th> </tr> <tr> <td><a href="#" title="CSS3 @keyframes 规则">@keyframes</a></td> <td>规定动画。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation 属性">animation</a></td> <td>所有动画属性的简写属性，除了 animation-play-state 属性。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-name 属性">animation-name</a></td> <td>规定 @keyframes 动画的名称。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-duration 属性">animation-duration</a></td> <td>规定动画完成一个周期所花费的秒或毫秒。默认是 0。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-timing-function 属性">animation-timing-function</a></td> <td>规定动画的速度曲线。默认是 "ease"。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-delay 属性">animation-delay</a></td> <td>规定动画何时开始。默认是 0。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-iteration-count 属性">animation-iteration-count</a></td> <td>规定动画被播放的次数。默认是 1。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-direction 属性">animation-direction</a></td> <td>规定动画是否在下一周期逆向地播放。默认是 "normal"。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 animation-play-state 属性">animation-play-state</a></td> <td>规定动画是否正在运行或暂停。默认是 "running"。</td> <td>3</td> </tr> </tbody></table>

## 源码

本文中所用例子源码参见
<https://github.com/waylau/css3-tutorial> 中 `samples` 目录下的 animation.html、animation_2.html