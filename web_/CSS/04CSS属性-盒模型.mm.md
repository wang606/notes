# CSS属性-盒模型

> CSS盒模型代表网站的设计和布局。【网页的每一个元素都是一个盒子】由**外边框（margin）**，**边框（border）**，**内边距（填充）（padding）**和**实际内容**组成。属性以相同的顺序工作：

\![0001]\(img/0001.jpg "CSS盒模型")

![0001](https://i.loli.net/2021/01/28/PfvxgUMWR5GF6VX.jpg "CSS盒模型")

### 元素的总宽度

\![0002]\(img/0002.jpg "元素的总宽度")

![0002](https://i.loli.net/2021/01/28/kF4YqbuPT7ygd5X.jpg "元素的总宽度")

> 在盒模型中设置的背景颜色将覆盖内容区域及填充区域（padding）。

### 元素的总高度

\![0003]\(img/0003.jpg "元素的总高度")

![0003](https://i.loli.net/2021/01/28/magCV87iqUvFEdb.jpg "元素的总高度")

> 遇到内容div想要居中与外部div中，可以使用`margin: 0 auto; `这样会根据内部div宽度自动填充左右两侧的margin值以达到居中效果。 

## border属性

> `border: border-width | border-style | border-color; `

```html
<html>
    <head>
        <style type="text/css">
            p {
                padding: 10px; 
                border: 5px solid green;
            }
        </style>
    </head>
    <body>
        <p>
            I am surrounded by green, right?
        </p>
    </body>
</html>
```

### border-style属性

> `border-style: none | solid | dotted | dashed | double | groove | ridge | inset | outset | hidden; `

```html
<html>
    <head>
        <style type="text/css">
            p.none {
                border-style: none;
            }
            p.solid {
                border-style: solid;
            }
            p.dotted {
                border-style: dotted;
            }
            p.dashed {
                border-style: dashed;
            }
            p.double {
                border-style: double;
            }
            p.groove {
                border-style: groove;
            }
            p.ridge {
                border-style: ridge;
            }
            p.inset {
                border-style: inset;
            }
            p.outset {
                border-style: outset;
            }
            p.hidden {
                border-style: hidden;
            }
        </style>
    </head>
    <body>
        <p class="none">
            none
        </p>
        <p class="solid">
            solid
        </p>
        <p class="dotted">
            dotted
        </p>
        <p class="dashed">
            dashed
        </p>
        <p class="double">
            double
        </p>
        <p class="groove">
            groove
        </p>
        <p class="ridge">
            ridge
        </p>
        <p class="inset">
            inset
        </p>
        <p class="outset">
            outset
        </p>
        <p class="hidden">
            hidden
        </p>
    </body>
</html>
```

> 可以使用以下属性为不同的边指定不同的边框：
>
> - border-top-style：上边框
> - border-right-style：右边框
> - border-bottom-style：下边框
> - border-left-style：左边框

```html
<p style="border-top-style: dashed; ">
    w3cschool
</p>
```

<p style="border-top-style: dashed; ">
    w3cschool
</p>

### border-width属性

> border-width设置边框的宽度。

```html
<html>
    <head>
        <style type="text/css">
            p.first {
                padding: 10px;
                border-style: solid;
                border-width: 2px;
            }
            p.second {
                padding: 10px;
                border-style: solid;
                border-width: 5px;
            }
        </style>
    </head>
    <body>
        <p class="first">
            w3xschool
        </p>
        <p class="second">
            w3cschool
        </p>
    </body>
</html>
```

<p style="border: 2px solid; ">w3cschool</p>

<p style="border: 5px solid; ">w3cschool</p>

### border-color属性

> 可以使用颜色名称关键词，RGB或十六进制值定义元素的边框颜色。

```html
<html>
    <head>
    	<style type="text/css">
            p.first, p.second, p.third {
                padding: 10px; 
                border-style: solid; 
                border-width: 2px; 
            }
            p.first {
                border-color: blue;
            }
            p.second {
                border-color: #FF6600;
            }
            p.third {
                border-color: rgb(0, 153, 0); 
            }
        </style>
    </head>
    <body>
        <p class="first">
            blue
        </p>
        <p class="second">
            #FF6600
        </p>
        <p class="third">
            rgb(0, 153, 0)
        </p>
    </body>
</html>
```

<p style="border: 2px solid blue; ">blue</p>

<p style="border: 2px solid #FF6600; ">#FF6600</p>

<p style="border: 2px solid rgb(0, 153, 0); ">rgb(0, 153, 0)</p>

## CSS的宽度和高度

```html
<html>
    <head>
        <style type="text/css">
            div {
                border: 5px solid green; 
                width: 80%;
                height: 90px;
            }
        </style>
    </head>
    <body>
        <div>
            I am <b>80%</b> wide and <b>100px</b> tall.
        </div>
    </body>
</html>
```

<div style="border: 5px solid green; width: 80%; height: 90px; ">I am <b>80%</b> wide and <b>100px</b> tall.</div>

### 最小最大尺寸

```html
<html>
    <head>
        <style type="text/css">
            p.first {
                border: 5px solid green;
                min-height: 100px;
            }
            p.second {
                border: 5px solid green;
                max-width: 100px; 
            }
            p.third {
                border: 5px solid green;
                max-height: 50px; 
                max-width: 100px;
            }
        </style>
    </head>
    <body>
        <p class="first">
            min-height is 100px.
        </p>
        <p class="second">
            max-width is 100px.
        </p>
        <p class="third">
            max-height is 50px and max-width is 100px.
        </p>
    </body>
</html>
```

<p style="border: 5px dashed gray; min-height: 100px; ">min-height is 100px.</p>

<p style="border: 5px dashed gray; max-width: 100px; ">max-width is 100px.</p>

<p style="border: 5px dashed gray; max-width: 100px; max-height: 50px; ">man-height is 50px and max-width is 100px.</p>

