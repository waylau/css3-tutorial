文本效果
====

CSS3 文本效果是这样一个术语用来在正常的文本中实现一些额外的特性。

主要是两个属性的 CSS3 文本效果,如下:

* text-shadow
* word-wrap

**注意:**Internet Explorer 10, Firefox,Chrome, Safari, 和 Opera支持text-shadow 属性。所有的主流浏览器支持自动换行（word-wrap）属性。Internet Explorer 9及更早IE版本不支持 text-shadow 属性

## text-shadow

文本阴影。
您指定了水平阴影，垂直阴影，模糊的距离，以及阴影的颜色：

    .text-shadow {
        text-shadow: 10px 10px 10px #6AAFCF;
    }


## word-wrap

换行。
CSS3中，自动换行属性允许您强制文本换行 - 即使这意味着分裂它中间的一个字：

    .word-wrap {
        word-wrap: break-word;
        width: 150px;
        border: 1px solid #ff0000;
    }

## 属性

<table class="reference"> <tbody><tr> <th style="width:25%;">属性</th> <th>描述</th> <th style="width:5%;">CSS</th> </tr> <tr> <td><a href="#" title="CSS3 hanging-punctuation 属性">hanging-punctuation</a></td> <td>规定标点字符是否位于线框之外。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 punctuation-trim 属性">punctuation-trim</a></td> <td>规定是否对标点字符进行修剪。</td> <td>3</td> </tr> <tr> <td>text-align-last</td> <td>设置如何对齐最后一行或紧挨着强制换行符之前的行。</td> <td>3</td> </tr> <tr> <td>text-emphasis</td> <td>向元素的文本应用重点标记以及重点标记的前景色。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 text-justify 属性">text-justify</a></td> <td>规定当 text-align 设置为 "justify" 时所使用的对齐方法。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 text-outline 属性">text-outline</a></td> <td>规定文本的轮廓。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 text-overflow 属性">text-overflow</a></td> <td>规定当文本溢出包含元素时发生的事情。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 text-shadow 属性">text-shadow</a></td> <td>向文本添加阴影。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 text-wrap 属性">text-wrap</a></td> <td>规定文本的换行规则。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 word-break 属性">word-break</a></td> <td>规定非中日韩文本的换行规则。</td> <td>3</td> </tr> <tr> <td><a href="#" title="CSS3 word-wrap 属性">word-wrap</a></td> <td>允许对长的不可分割的单词进行分割并换行到下一行。</td> <td>3</td> </tr> </tbody></table>

## 源码

本文中所用例子源码参见
<https://github.com/waylau/css3-tutorial> 中 `samples` 目录下的 texteffects.html