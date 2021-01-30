# CSS定位与布局

## display属性

> display属性决定了盒模型的行为方式。
>
> `display: none; `让标签消失（隐藏元素并脱离文档流）。
>
> `display: inline; `内联元素（内联标签）。
>
> `display: block; `块级元素（块级标签）。
>
> `display: inline-block; `既有inline的属性也有block属性。
>
> display还有很多其他的参数值，如：list-item, table, table-cell, table-column, grid等等。

### display: block; 

> block（块元素）是占用最大可用宽度的元素，默认情况下block元素自动填满其父元素宽度。
>
> block元素前后会带有换行符，可以设置width和height属性，但仍然独占一行。
>
> block元素也可以设置margin和padding属性。
>
> 常见的块级元素有：div，p，ul，ol，li，h1~h6等。

```html
<html>
    <head>
        <style type="text/css">
            span {
                display: block; 
            }
        </style>
    </head>
    <body>
        <span>First Paragraph.</span>
        <span>Second Paragraph.</span>
        <span>Third Paragraph.</span>
        <span>Fourth Paragraph.</span>
        <span>Fifth Paragraph.</span>
    </body>
</html>
```

> 设置元素的display属性只会改变元素的显示方式，而不会改变元素的类型。故带有`display: block; `的内联元素不允许在其中包含其他块元素。

### display: inline; 

> inline元素默认的宽度是自身内容的宽度，不会独占一行。
>
> inline元素设置width和height属性无效。
>
> inline元素的margin和padding属性，水平方向可产生边距效果，但垂直方向无效。

```html
<html>
    <head>
        <style type="text/css">
            p {
                display: inline; 
            }
        </style>
    </head>
    <body>
        <p>
            First Paragraph.
        </p>
        <p>
            Second Paragraph.
        </p>
        <p>
            Third Paragraph.
        </p>
        <p>
            Fourth Paragraph.
        </p>
        <p>
            Fifth Paragraph.
        </p>
    </body>
</html>
```

### display: none; 

> none属性不占用任何空间。其子元素也无法显示。
>
> none属性会引起页面重绘和回流，脱离文档。

```html
<html>
    <head>
        <style type="text/css">
            h1 {
                display: none; 
            }
        </style>
    </head>
    <body>
        <h1>
            I am hiden since my display has been set to none.
        </h1>
        <p>
            Just me.Yes, it is my show time.
        </p>
    </body>
</html>
```

### display: inline-block; 

> 不独占一行。
>
> 能够改变height和width值
>
> 可以设置padding和margin的各个值。

## visibility属性

> visible：【默认】可见。
>
> hidden：不可见。但占有空间。
>
> - `display: none; `不占空间；浏览器不解析；产生回流和重绘；
> - `visibility: hidden; `占空间；浏览器会解析；只重绘不回流；

## position定位

> position属性指定一个元素（静态的，相对的，绝对或固定）的定位方法的类型。
>
> `position: absolute | fixed | relative | static | inherit; `
>
> - absolute：生成绝对定位的元素，相对于static定位以外的第一个父元素进行定位。元素的位置通过“top、right、bottom、left”属性进行规定。
> - fixed：生成固定定位的元素，相对于浏览器窗口进行定位。元素的位置通过“top、right、bottom、left”属性进行规定。
> - relative：生成相对定位的元素，相对其正常位置进行定位。
> - static：【默认】无特殊定位。
> - inherit：从父元素继承。

## z-index属性

> z-index属性指定元素的堆栈顺序（通过z-index的值可以决定那个元素应该放置在其他元素的前面或后面）。
>
> 当元素位于正常流程顺序之外时（受position等属性影响时），它们可以重叠于其他元素。

```html
<html>
    <head>
        <style type="text/css">
            .blue {
                background-color: #8ec4d0; 
                margin-bottom: 15px; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
            }
            .red {
                background-color: #ff4d4d; 
                position: relative; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
                margin: -50px 50px; 
            }
        </style>
    </head>
    <body>
        <div class="blue">
            blue<br/>(w3cschool)
        </div>
        <div class="red">
            red<br/>(w3cschool)
        </div>
    </body>
</html>
```

<div style="background-color: #8ec4d0; 
                margin-bottom: 15px; 
                width: 120px; 
                height: 120px; 
                color: #fff; ">
    blue<br/>(w3cschool)
</div>

<div style="background-color: #ff4d4d; 
                position: relative; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
                margin: -50px 50px; ">
    red<br/>(w3cschool)
</div>



> 红框与蓝框重叠，红框位于蓝框上方，因为红框是后加载的。设置z-index属性可以改变这个顺序。

```html
<html>
    <head>
        <style type="text/css">
            .blue {
                background-color: #8ec4d0; 
                margin-bottom: 15px; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
                z-index: 3; 
            }
            .red {
                background-color: #ff4d4d; 
                position: relative; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
                margin: -50px 50px; 
                z-index: 2; 
            }
        </style>
    </head>
    <body>
        <div class="blue">
            blue<br/>(w3cschool)
        </div>
        <div class="red">
            red<br/>(w3cschool)
        </div>
    </body>
</html>
```

<div style="background-color: #8ec4d0; 
                margin-bottom: 15px; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
                z-index: 3;">
    blue<br/>(w3cschool)
</div>

<div style="background-color: #ff4d4d; 
                position: relative; 
                width: 120px; 
                height: 120px; 
                color: #fff; 
                margin: -50px 50px; 
                z-index: 2; ">
    red<br/>(w3cschool)
</div>



> z-index仅适用于定位元素absolute, relative, fixed!

## float属性

> float属性指定一个盒子（元素）是否应该浮动。使用float，可以将元素向左或向右推，以允许其他元素环绕它。
>
> float通常与图像一起使用，但在处理布局时也很有用。
>
> `float: left | right | none; `
>
> - left, right会使元素向左或向右浮动。
> - none确保元素不进行浮动。

```html
<html>
    <head>
        <style type="text/css">
            img {
                float: right; 
            }
        </style>
    </head>
    <body>
        <p><img src="https://7nsts.w3cschool.cn/images/w3c/header-logo.png" />
This paragraph has an image that is floated to the <strong>right.</strong> 
It is highly recommended to add a margin to images so that the text does 
not get too close to the image. If you want your text to be easily read, you 
should always add a few pixels between words and borders, images, 
and other content. 
</p >
    </body>
</html>
```

<p><img src="https://7nsts.w3cschool.cn/images/w3c/header-logo.png" style="float: right; " />
This paragraph has an image that is floated to the <strong>right.</strong> 
It is highly recommended to add a margin to images so that the text does 
not get too close to the image. If you want your text to be easily read, you 
should always add a few pixels between words and borders, images, 
and other content. 
</p >

### 元素相邻

> 如果连续放置几个浮动的元素，那么如果有足够的空间，他们将**相互浮动**。

```html
<html>
    <head>
        <style type="text/css">
            img {
                float:left; 
                width: 120px; 
                margin-right: 10px; 
            }
            p {
                width: 150px; 
                float: left; 
            }
        </style>
    </head>
    <body>
        <p>
            <img src="https://7nsts.w3cschool.cn/images/w3c/header-logo.png" />
            哦， 这是w3cschool!
        </p>
    </body>
</html>
```

<p style="float: left; ">
<img src="https://7nsts.w3cschool.cn/images/w3c/header-logo.png" style="float: left; "/>
哦， 这是w3cschool!
</p>



## 清除float

> 元素设置了float属性后会使后面的元素都受其影响，将环绕在其周围。可以使用clear属性。
>
> `clear: both | left | right | none; `

```html
<html>
    <head>
        <style type="text/css">
            p {
                height: 20px; 
                border: 1px solid green; 
            }
            .floating {
                float: right; 
            }
            .clear {
                clear: both; 
            }
        </style>
    </head>
    <body>
        <p>
            I am not affected by the floating image, since I am above of it.
        </p>
        <div class="floating">
            <img src="https://7nsts.w3cschool.cn/images/w3c/header-logo.png" />
        </div>
        <p>
            I am affected by the floating image, since I am below of it.
        </p>
        <p class="clear">
            I am not affected by the floating image, since I clear the affection of the floating image. 
        </p>
    </body>
</html>
```

## overflow属性

> overflow属性指定如果内容溢出一个元素的框会发生什么。

```html
<html>
    <head>
        <style type="text/css">
            div {
                width: 150px; 
                height: 150px; 
                background-color: LightBlue; 
                float: left; 
            }
        </style>
    </head>
    <body>
        <div>
            这个文本在div元素里面，他有一个天蓝色的背景颜色，并浮动在左侧。<br/>我们设定了一个具体的div元素的高度和宽度，如你所见，我溢出了。。。
        </div>
    </body>
</html>
```

<div style="width: 150px; height: 150px; background-color: LightBlue; float: left;">
      这个文本在div元素里面，他有一个天蓝色的背景颜色，并浮动在左侧。<br/>我们设定了一个具体的div元素的高度和宽度，如你所见，我溢出了。。。
</div>











> `overflow: visible | hidden | scroll | auto; `
>
> - visible：【默认】内容不会被修剪，会呈现在元素框之外。
> - hidden：内容被修剪，并且其与内容是不可见。
> - scroll：内容被修剪，但是浏览器会显示滚动条以便查看其余内容（不溢出也会有滚动条）
> - auto：如果内容被修剪（如文字溢出时），浏览器才会显示滚动条以便查看其余内容。

```html
<html>
    <head>
        <style type="text/css">
            div {
                width: 150px; 
                height: 150px; 
                background-color: LightBlue; 
                float: left; 
                overflow: scroll; 
            }
        </style>
    </head>
    <body>
        <div>
            这个文本在div元素里面，他有一个天蓝色的背景颜色，并浮动在左侧。<br/>我们设定了一个具体的div元素的高度和宽度，如你所见，我溢出了。。。
        </div>
    </body>
</html>
```

<div style="width: 150px; height: 150px; background-color: LightBlue; float: left; overflow: scroll; ">
      这个文本在div元素里面，他有一个天蓝色的背景颜色，并浮动在左侧。<br/>我们设定了一个具体的div元素的高度和宽度，如你所见，我溢出了。。。
</div>







