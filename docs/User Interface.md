UI
====

增加了一些新的用户界面特性来调整元素尺寸，框尺寸和外边框。

在本章中，您将了解以下的用户界面属性：

* resize
* box-sizing
* outline-offset

**注意：**Firefox、Chrome 以及 Safari 支持 resize 属性。
Internet Explorer、Chrome、Safari 以及 Opera 支持 box-sizing 属性。Firefox 需要前缀 -moz-。
所有主流浏览器都支持 outline-offset 属性，除了 Internet Explorer。

## resize

resize 属性指定一个元素是否应该由用户去调整大小。可以使用  `resize:both`， `resize:vertical` 或者 `resize:horizontal`，用来分别设置元素是可以水平、垂直调整，垂直调整，水平调整。

例子

    .div-both {
        border: 1px solid green;
        margin-top: 20px;
        padding: 15px 30px;
        width: 250px;
        resize: both;
        overflow: auto;
    }

    .div-horizontal {
        border: 1px solid green;
        margin-top: 20px;
        padding: 15px 30px;
        width: 250px;
        resize: horizontal;
        overflow: auto;
    }

    .div-vertical {
        border: 1px solid green;
        margin-top: 20px;
        padding: 15px 30px;
        width: 250px;
        resize: vertical;
        overflow: auto;
    }

## box-sizing

box-sizing 允许您以确切的方式定义适应某个区域的具体内容

例子

    .box-sizing {
        box-sizing: border-box;
        -moz-box-sizing: border-box; /* Firefox */
        width: 50%;
        border: 1em solid red;
        float: left;
    }

## outline-offset

outline-offset 属性对轮廓进行偏移，并在超出边框边缘的位置绘制轮廓。

轮廓与边框有两点不同：

* 轮廓不占用空间
* 轮廓可能是非矩形

例子

    .outline-offset {
        width: 180px;
        height: 80px;
        border: 1px solid red;
        outline: 1px solid green;
        outline-offset: 20px;
    }

## 属性

<table class="reference"> <tbody><tr> <th width="28%" align="left">属性</th> <th width="67%" align="left">说明</th> <th width="5%" align="left">CSS</th> </tr> <tr> <td><a href="#">appearance</a></td> <td>允许您使一个元素的外观像一个标准的用户界面元素</td> <td>3</td> </tr> <tr> <td><a href="#">box-sizing</a></td> <td>允许你以适应区域而用某种方式定义某些元素</td> <td>3</td> </tr> <tr> <td><a href="#">icon</a></td> <td>Provides the author the ability to style an element with an iconic equivalent</td> <td>3</td> </tr> <tr> <td><a href="#">nav-down</a></td> <td>指定在何处使用箭头向下导航键时进行导航</td> <td>3</td> </tr> <tr> <td><a href="#">nav-index</a></td> <td>指定一个元素的Tab的顺序</td> <td>3</td> </tr> <tr> <td><a href="#">nav-left</a></td> <td>指定在何处使用左侧的箭头导航键进行导航</td> <td>3</td> </tr> <tr> <td><a href="#">nav-right</a></td> <td>指定在何处使用右侧的箭头导航键进行导航</td> <td>3</td> </tr> <tr> <td><a href="#">nav-up</a></td> <td>指定在何处使用箭头向上导航键时进行导航</td> <td>3</td> </tr> <tr> <td><a href="#">outline-offset</a></td> <td>外轮廓修饰并绘制超出边框的边缘</td> <td>3</td> </tr> <tr> <td><a href="#">resize</a></td> <td>指定一个元素是否是由用户调整大小</td> <td>3</td> </tr> </tbody></table>

## 源码

本文中所用例子源码参见
<https://github.com/waylau/css3-tutorial> 中 `samples` 目录下的 userinterface.html