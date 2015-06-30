边框
====

CSS3 Border（边框）主要有以下属性：

* border-radius
* box-shadow
* border-image

**注意：**Internet Explorer 9+ 支持 border-radius 和 box-shadow 属性。Firefox、Chrome 以及 Safari 支持所有新的边框属性。
对于 border-image，Safari 5 以及更老的版本需要前缀 -webkit-。
Opera 支持 border-radius 和 box-shadow 属性，但是对于 border-image 需要前缀 -o-

## border-radius （圆角边框）

在 CSS3 中，border-radius 属性用于创建圆角

	.border_radius {
	    border: 2px solid;
	    font-size: 14px;
	    color: #ffffff;
	    font-weight: bold;
	    padding: 10px;
	    background: #6AAFCF;
	    border-radius: 25px;
	    -moz-border-radius: 25px; /* For Firefox Browser */
	    -webkit-border-radius: 25px; /* For Safari and Google Chrome Browser */
	    -o-border-radius: 25px /* For Opera Browser */
	}

## box-shadow （边框阴影）

在 CSS3 中，box-shadow 用于向方框添加阴影：

    .box_shadow {
        font-size: 14px;
        color: #ffffff;
        font-weight: bold;
        padding: 10px;
        background: #6AAFCF;
        -moz-box-shadow: 15px 15px 5px #888245; /* For Firefox/Mozilla */
        -webkit-box-shadow: 15px 15px 5px #888245; /* For Google Chrome and Safari */
        -o-box-shadow: 15px 15px 5px #888245; /* For Opera */
        box-shadow: 15px 15px 5px #888245;
    }

## border-image （边框图片）

通过 CSS3 的 border-image 属性，您可以使用图片来创建边框：

    .border_image {
        border-width: 15px;
        -moz-border-image: url(/images/border.png) 30 30 round; /* Firefox */
        -webkit-border-image: url(/images/border.png) 30 30 round; /* Safari and Chrome */
        -o-border-image: url(/images/border.png) 30 30 round; /* Opera */
        border-image: url(/images/border.png) 30 30 round;
    }

## 源码

本文中所用例子源码参见
<https://github.com/waylau/css3-tutorial> 中 `samples` 目录下的 border.html