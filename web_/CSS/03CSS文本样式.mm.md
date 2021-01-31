# CSS文本样式

## font-family属性

> **font-family**属性指定元素的字体。
>
> 用**逗号**分隔每个值，以表明它们是可选项。
>
> 如果一个字体的名字不止一个单词，那么必须用引号。在HTML"style"属性中，必须使用单引号。

```html
<!-- html part -->
<p class="serif">
    This is a paragraph shown in serif font.
</p>
<p class="sansserif">
    This is a paragraph shown in sansserif font.
</p>
<p class="monospace">
    This is a paragraph shown in monospace font.
</p>
<p class="cursive">
    This is a paragraph shown in cursive font.
</p>
<p class="fantasy">
    This is a paragraph shown in fantasy font.
</p>
```

```CSS
/* CSS part */
p.serif {
    font-family: "Times New Roman", Times, serif;
}
p.sansserif {
    font-family: Helvetica, Arial, sansserif;
}
p.monospace {
    font-family: "Courier New", Courier, monospace;
}
p.cursive {
    font-family: Florence, cursive;
}
p.fantasy {
    font-family: Blippo, fantasy;
}
```

## font-size属性

> font-size属性用于设置字体的大小，设置网页字体大小的方法之一是**使用关键字**，如：xx-small，small，medium，large，larger，etc等。

```html
<!-- HTML part -->
<p class="small">
    Paragraph text set to be small.
</p>
<p class="medium">
    Paragraph text set to be medium.
</p>
<p class="large">
    Paragraph text set to be large.
</p>
<p class="xlarge">
    Paragraph text set to be xlarge.
</p>
<p class="px">
    Paragraph text set to be 20px.
</p>
<p class="rem">
    Paragraph text set to be 2rem.
</p>
```

```CSS
/* CSS part */
p.small {
    font-size: small;
}
p.medium {
    font-size: medium;
}
p.large {
    font-size: large;
}
p.xlarge {
    font-size: x-large;
}
p.px {
    font-size: 20px;
}
p.rem {
    font-size: 2rem;
}
```

> 可以使用**像素（px）**或**相对尺寸单位（em）**或**pt**数值来操作字体大小。
>
> px特点：
>
> - IE无法调整以px为单位的字体的大小；
> - Firefox可以调整px和em，rem
>
> em（font size of the element）是指相对于父元素的字体大小的单位，如果你没有在页面上的任何位置设置字体大小，那么这是浏览器的默认大小，即16px。现指的是字符宽度的倍数，用法类似百分比，如0.8em，1.2em等。
>
> em特点：
>
> - em的值并不是固定的，会继承父级元素的字体大小。
>
> 所有未经调整的浏览器都符合：1em=16px。为了简化font-size的换算，需在CSS中的body选择器中声明Font-size=62.5%，这就使1em=10px。

## font-style属性

> font-style属性用于定义字体风格，加设置斜体、倾斜或正常字体。
>
> `font-style: normal | italic | oblique; `
>
> normal: 正常字体。 
>
> italic: 斜体。【对于有斜体变量的特殊字体有效】
>
> oblique: 倾斜字体。

```html
<!-- HTML part -->
<p class="normal">
    I am normal!
</p>
<p class="italic">
    I am italics.
</p>
<p class="oblique">
    I am oblique.
</p>
<p>
    <i>I am in "&lt;i&gt;".</i>
</p>
```

```CSS
/* CSS part */
p.normal {
    font-style: normal;
}
p.italic {
    font-style: italic;
}
p.oblique {
    font-style: oblique;
}
```

## font-weight属性

> font-weight控制文本的粗细。
>
> `font-weight: normal | bold | bolder | lighter; `
>
> 根据文本的厚度，也可以使用从100（细）到900（粗）的数字来定义字体粗细。400对应normal，700对应bold。

```html
<!-- HTML part -->
<p class="lighter">
    This is a font with a "lighter" weight.
</p>
<p>
    This is a font with a "normal" weight.
</p>
<p class="bold">
    This is a font with a "bold" weight.
</p>
<p class="bold_">
    This is a font with a "700" weight.
</p>
<p class="bolder">
    This is a font with a "bolder" weight.
</p>
<p>
    <b>This is a font with a "&lt;b&gt;" weight.</b>
</p>
```

```CSS
/* CSS part */
p.lighter {
    font-weight: lighter;
}
p.bold {
    font-weight: bold;
}
p.bold_ {
    font-weight: 700;
}
p.bolder {
    font-weight: bolder;
}
```

## font-variant属性

> font-variant属性允许你将字体转换为所有小型大写字母。
>
> `font-variant: normal | small-caps | inherit; `

```html
<!-- HTML part -->
<p class="normal">
    Paragraph font variant set to normal.
</p>
<p class="samll">
    Paragraph font variant set to small-caps.
</p>
```

```CSS
/* CSS part */
p.normal {
    font-variant: normal;
}
p.small {
    font-variant: small-caps;
}
```

## color

> color属性用于指定文本的颜色。

```html
<html>
    <head>
        <style>
            p.red {
                color: rgb(255, 0, 0);
            }
            p.blue {
                color: #0000FF;
            }
            p.green {
                color: green;
            }
        </style>
    </head>
    <body>
        <p class="red">
            I am red with rgb(255, 0, 0).
        </p>
        <p class="blue">
            I am blue with #0000FF.
        </p>
        <p class="green">
            I am green with green.
        </p>
    </body>
</html>
```

## text-align属性

> text-align属性指定元素中文本的水平对齐方式。
>
> `text-align: left | right | center | justify; `
>
> justify实现两端对齐文本效果；inherit规定从父元素继承text-align属性的值。

```html
<html>
    <head>
        <style type="text/css">
            p.left {
                text-align: left;
            }
            p.right {
                text-align: right;
            }
            p.center {
                text-align: center;
            }
        </style>
    </head>
    <body>
        <p class="left">
            <b>w3cschool</b>
        </p>
        <p class="right">
            <b>w3cschool</b>
        </p>
        <p class="center">
            <b>w3cschool</b>
        </p>
    </body>
</html>
```

## vertical-align属性

> vertical-align属性设置元素的垂直对齐。
>
> `vertical-align: top | middle | bottom; `

```html
<html>
    <head>
        <style type="text/css">
            td.top {
                vertical-align: top;
            }
            td.middle {
                vertical-align: middle;
            }
            td.bottom {
                vertical-align: bottom;
            }
        </style>
    </head>
    <body>
        <table border="1" cellpadding="2" cellspacing="0" style="height: 150px; ">
            <td class="top">Top</td>
            <td class="middle">Middle</td>
            <td class="bottom">Bottom</td>
        </table>
    </body>
</html>
```

> vertical-align属性还包含以下值：
>
> - baseline: 使元素的基线与父元素的基线对齐。
> - sub: 使元素的基线与父元素的下标基线对齐。
> - super: 使元素的基线与父元素的上标基线对齐。
> - px: 使元素的基线对齐到父元素的基线之上的给定长度。可以是负数。
> - 可以使用%（百分比）、pt（点）、cm（厘米）值来代替px值。

```html
<html>
    <head>
        <style type="text/css">
            span.baseline {
                vertical-align: baseline;
            }
            span.sub {
                vertical-align: sub;
            }
            span.super {
                vertical-align: super;
            }
            span.pixel {
                vertical-align: -10px;
            }
        </style>
    </head>
    <body>
        <p>
            This is a <span class="baseline">w3cschool</span> example.
        </p>
        <p>
            This is a <span class="sub">w3cschool</span> example.
        </p>
        <p>
            This is a <span class="super">w3cschool</span> example.
        </p>
        <p>
            This is a <span class="pixel">w3cschool</span> example.
        </p>
    </body>
</html>
```

> vertical-align属性对所有元素的行为都不一样。

```html
<html>
    <head>
        <style type="text/css">
            .main {
                height: 150px; 
                width: 400px; 
                background-color: LightSkyBlue; 
                display: inline-table;
            }
            .paragraph {
                display: table-cell;
                vertical-align: middle;
            }
        </style>
    </head>
    <body>
        <div class="main">
            <div class="paragraph">
                w3cschool
            </div>
        </div>
    </body>
</html>
```

> display: inline-table; 和display: table-cell; 使用样式来使垂直对齐属性能在div中起效果。

## text-decoration属性

> text-decoration属性用于指定文本将如何装饰。
>
> text-decoration属性是由以下三种属性的简写：
>
> - text-decoration-line：线条类型
> - text-decoration-color：线条颜色
> - text-decoration-style：线条样式
>
> `text-decoration: none | inherit | overline | underline | line-through | blink; `
>
> - none：默认值，正常文本
> - inherit：从父元素继承此属性
> - overline：在文本上方绘制水平线
> - underline：在文本下方绘制水平线
> - line-through：\<s>
> - blink：文本闪烁。【被大多数浏览器弃用】

```html
<html>
    <head>
        <style type="text/css">
            p.none {
                text-decoration: none;
            }
            p.inherit {
                text-decoration: inherit;
            }
            p.overline {
                text-decoration: overline;
            }
            p.underline {
                text-decoration: underline;
            }
            p.line-through {
                text-decoration: line-through;
            }
            /* 可将overline, underline, line-through组合起来 */
            p.mixed {
                text-decoration: overline, underline, line-through; 
            }
        </style>
    </head>
    <body>
        <p class="none">
            w3cschool
        </p>
        <p class="inherit">
            w3cschool
        </p>
        <p class="overline">
            w3cschool
        </p>
        <p class="underline">
            w3cschool
        </p>
        <p class="line-through">
            w3cschool
        </p>
        <p class="mixed">
            w3cschool
        </p>
    </body>
</html>
```

## text-indent属性

> text-indent属性规定文本中首行文本的缩进。
>
> 属性值是长度（px、pt、cm、em等），%和inherit。
>
> 内联对象要使用该属性必须先使该对象表现为**块级**或**内联块级**。

```html
<html>
    <head>
        <style type="text/css">
            p.right {
                text-indent: 60px;
            }
            p.left {
                text-indent: -40px;
            }
        </style>
    </head>
    <body>
        <p class="right">
            使用<b>text-indent</b>让文本向右缩进了60px。
        </p>
        <p>
            正常文本。
        </p>
        <p class="left">
            设置负值让文本向左缩进了40px。
        </p>
    </body>
</html>
```

> 如果使用负值那么首行会被缩进到左边。
>
> text-indent属性用于定义**块级元素**中第一个**内容行**的缩进。这最常用于建立一个**“标签页”**效果。允许指定负值，这会产生一种**“悬挂缩进”**的效果。

## text-shadow属性

> text-shadow为文本添加阴影。
>
> `text-shadow: h-shadow v-shadow blur color; `
>
> - h-shadow：必需。水平阴影的位置。允许负值。
> - v-shadow：必需。垂直阴影的位置。允许负值。
> - blur：可选。模糊的距离。
> - color：可选。阴影的颜色。

```html
<html>
    <head>
        <style type="text/css">
            h1 {
                color: blue;
                font-size: 30px;
                text-shadow: 5px 2px 4px red;
            }
        </style>
    </head>
    <body>
        <h1>
            w3cschool
        </h1>
    </body>
</html>
```

<h1 style="color: blue; font-size: 30px; text-shadow: 5px 2px 4px red; ">w3cschool</h1>

```html
<html>
    <head>
        <style type="text/css">
            h1 {
                font-size: 20pt;
                text-shadow: rgba(0, 255, 255, 1) -1px -2px 0.5em;
            }
        </style>
    </head>
    <body>
        <h1>
            w3cschool
        </h1>
    </body>
</html>
```

<h1 style="font-size: 20pt; text-shadow: rgba(0, 255, 255, 1) -1px -2px 0.5em; ">w3cschool</h1>

## text-transform属性

> text-transform属性控制文本的大小写。
>
> `text-transform: capitalize | uppercase | lowercase; `
>
> - capitalize可以实现文本中的每个单词以大写字母开头。
> - uppercase：全部大写。
> - lowercase：全部小写。

```html
<html>
    <head>
        <style type="text/css">
            p.capitalize {
                text-transform: capitalize;
            }
        </style>
    </head>
    <body>
        <p class="capitalize">
            The value capitalize transforms the first character in each word to uppercase; all other characters remain unaffected.
        </p>
    </body>
</html>
```

## letter-spacing属性

> letter-spacing属性用于设置文本中字符之间的间距。

```html
<html>
    <head>
        <style type="text/css">
            p.normal {
                letter-spacing: normal;
            }
            p.positive {
                letter-spacing: 4px;
            }
            p.negative {
                letter-spacing: -1.5px; 
            }
        </style>
    </head>
    <body>
        <p class="normal">
            w3cschool
        </p>
        <p class="positive">
            w3cschool
        </p>
        <p class="negative">
            w3cschool
        </p>
    </body>
</html>
```

## word-spacing属性

> word-spacing属性指定文本中单词之间的空格。

```html
<html>
    <head>
        <style type="text/css">
            p.normal {
                word-spacing: normal;
            }
            p.px {
                word-spacing: 40px;
            }
        </style>
    </head>
    <body>
        <p class="normal">
            This paragraph has no additional word-spacing applied.
        </p>
        <p class="px">
            This paragraph is word-spaced at 40px.
        </p>
    </body>
</html>
```

## white-space属性

> white-space可以设置**元素内**的**换行符**。
>
> `white-space: normal | inherit | nowrap | pre | pre-line | pre-wrap; `
>
> - normal：【默认】空白会被浏览器忽略。
> - inherit：规定从父元素继承。
> - nowrap：文本不换行直到\<br/>。【nowrap会屏蔽该元素中的所有换行符】
> - pre：文本支持所有的换行和空格。
> - pre-line：文本支持换行，忽略额外的空格。
> - pre-wrap：文本将在必要的时候或者行的结尾进行换行。

```html
<html>
    <head>
        <style type="text/css">
            p.normal {
                white-space: normal;
            }
            p.nowrap {
                white-space: nowrap;
            }
            p.pre {
                white-space: pre;
            }
            p.pre-line {
                white-space: pre-line;
            }
            p.pre-wrap {
                white-space: pre-wrap;
            }
        </style>
    </head>
    <body>
        <p class="normal">
            This paragraph has     //wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww//    multiple sapces              and  
            a line  break, it will turn this as    we used the normal value.
        </p>
        <p class="nowrap">
            This paragraph has     //wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww//    multiple sapces              and  
            a line  break, it will turn this as    we used the nowrap value.
        </p>
        <p class="pre">
            This paragraph has     //wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww//    multiple sapces              and  
            a line  break, it will turn this as    we used the pre value.
        </p>
        <p class="pre-line">
            This paragraph has     //wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww//    multiple sapces              and  
            a line  break, it will turn this as    we used the pre-line value.
        </p>
        <p class="pre-wrap">
            This paragraph has     //wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww//    multiple sapces              and  
            a line  break, it will turn this as    we used the pre-wrap value.
        </p>
    </body>
</html>
```

