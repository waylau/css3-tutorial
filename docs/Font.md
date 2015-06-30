字体
====

以前 CSS3 的版本，网页设计师不得不使用用户计算机上已经安装的字体。

使用 CSS3，网页设计师可以使用他/她喜欢的任何字体。

当你发现您要使用的字体文件时，只需简单的将字体文件包含在网站中，它会自动下载给需要的用户。

您所选择的字体在新的 CSS3 版本有关于`@font-face`规则描述。

您"自己的"的字体是在 CSS3 `@font-face` 规则中定义的。

**注意：**Internet Explorer 9+, Firefox, Chrome, Safari, 和 Opera 支持 WOFF (Web Open Font Format) 字体。

Firefox, Chrome, Safari, 和 Opera 支持 .ttf(True Type字体)和.otf(OpenType)字体字体类型）。

Chrome, Safari 和 Opera 也支持 SVG 字体/折叠。

Internet Explorer 同样支持 EOT (Embedded OpenType) 字体。

在 `@font-face` 规则中，您必须首先定义字体的名称（比如 FontAwesome ），然后指向该字体文件 fontawesome-webfont.woff 。

    @font-face {
        font-family: 'FontAwesome';
        src: url('fonts/fontawesome-webfont.woff');
    }

    .font6 {
        font-family: 'FontAwesome', sans-serif;
        font-size: 14px;
        color: pink;
        line-height: 1.3em;
    }

## 源码

本文中所用例子源码参见
<https://github.com/waylau/css3-tutorial> 中 `samples` 目录下的 font.html