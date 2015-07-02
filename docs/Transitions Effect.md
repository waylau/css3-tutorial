过渡效果
====

CSS3 过渡是元素从一种样式逐渐改变为另一种的效果。

尽管 CSS3 过渡效果是足够的过渡的一个元素,但是 text-transform 属性可以提高 CSS3 过渡效果的风格。

主要有四个属性的CSS3转换效果,已被描述如下:

* transition-property
* transition-duration
* transition-timing-function
* transition-delay

**注意：**Internet Explorer 10, Firefox, Opera, Chrome, 和Opera 支持transition 属性。Safari 需要前缀 -webkit-。Internet Explorer 9 以及更早的版本，不支持 transition 属性。Chrome 25 以及更早的版本，需要前缀 -webkit-

## transition-property

规定应用过渡的 CSS 属性的名称。

	transition-property: all;
	transition-property: none;
	transition-property: background-color;
	transition-property: background-color, height, width;


## transition-duration

定义过渡效果花费的时间。默认是 0。 时间单位可以是秒/毫秒。

	transition-duration: 2s;
	transition-duration: 1000ms;
	transition-duration: 1000ms, 2000ms;
	
## transition-timing-function

规定过渡效果的时间曲线。默认是 "ease"。

	transition-timing-function: ease;
	transition-timing-function: ease-in;
	transition-timing-function: ease-in-out;
	transition-timing-function: ease, linear;
	transition-timing-function: cubic-bezier(1.000, 0.835, 0.000, 0.945);

其中：

* linear：线性过渡。等同于贝塞尔曲线(0.0, 0.0, 1.0, 1.0)
* ease：平滑过渡。等同于贝塞尔曲线(0.25, 0.1, 0.25, 1.0)
* ease-in：由慢到快。等同于贝塞尔曲线(0.42, 0, 1.0, 1.0)
* ease-out：由快到慢。等同于贝塞尔曲线(0, 0, 0.58, 1.0)
* ease-in-out：由慢到快再到慢。等同于贝塞尔曲线(0.42, 0, 0.58, 1.0)
* step-start：等同于 steps(1, start)
* step-end：等同于 steps(1, end)
* steps(`<integer>[, [ start | end ] ]?`)：接受两个参数的步进函数。第一个参数必须为正整数，指定函数的步数。第二个参数取值可以是start或end，指定每一步的值发生变化的时间点。第二个参数是可选的，默认值为end。
* cubic-bezier(`<number>, <number>, <number>, <number>`)：特定的贝塞尔曲线类型，4个数值需在[0, 1]区间内


## transition-delay

规定过渡效果何时开始。默认是 0。

	transition-delay: 2s;
	transition-delay: 1000ms, 2000ms;
	transition-delay: -2s;

## 源码

本文中所用例子源码参见
<https://github.com/waylau/css3-tutorial> 中 `samples` 目录下的 transitions.html