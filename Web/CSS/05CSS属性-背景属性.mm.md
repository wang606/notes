# CSS属性-背景属性

## background-color属性

> background-color属性为元素设置一种纯色背景。这种颜色会填充元素的**内容**，**内边距**和**边框区域**，扩展到元素边框的**外边界（但不包括外边距）**。如果边框有透明部分（如虚线边框），会透过这些透明部分显示出背景色。

```html
<html>
    <head>
        <style type="text/css">
            body {
                margin: 20px;
                background-color: #87CEFA;
            }
            p {
                background-color: rgb(0, 153, 0); 
            }
        </style>
    </head>
    <body>
        <p>
            I am surrounded by LightSkyBlue, right?
        </p>
    </body>
</html>
```

<div style="background-color: #87CEFA; width: 90%; height: 40px; margin: 20px; ">
<p style="background-color: rgb(0, 153, 0); width: 100%">I am surrounded by LightSkyBlue, right?</p></div>

## background-image属性

> background-image属性为元素设置一个或多个背景图像。
>
> `background-image: url(图片路径)`
>
> 可设置一种可用的背景颜色备用。
>
> 默认情况下，背景图像放置在元素的左上角，并且垂直和水平重复以覆盖整个元素。

```html
<html>
    <head>
        <style type="text/css">
            body {
                background-image: url("img/0004.jpg");
                background-color: #e9e9e9; 
            }
        </style>
    </head>
    <body>
    </body>
</html>
```

## background-repeat属性

> background-repeat属性指定如何重复背景图像。
>
> - repeat：【默认】背景图像在横向和纵向平铺。
> - repeat-x：背景图像在横向上平铺。
> - repeat-y：背景图像在纵向上平铺。
> - no-repeat：不平铺。
> - round：背景图像自动缩放直至适应且填充满整个容器。（CSS3）
> - space：背景图像以相同的间距平铺且填充满整个容器或某个方向。（CSS3）

```html
<html>
    <head>
        <style type="text/css">
            body {
                background-image: url("img/0004.jpg"); 
                background-repeat: repeat-x; 
            }
            p {
                background-image: url("img/0004.jpg"); 
                background-repeat: inherit;
                margin-top: 100px; 
                padding: 40px; 
            }
        </style>
    </head>
    <body>
        <p>
            I am a paragraph.
        </p>
    </body>
</html>
```

## background-attachment属性

> background-attachment属性设置背景图像是固定的还是与页面的其余部分一起滚动。
>
> `background-attachment: scroll | fixed | inherit; `
>
> - scroll：【默认】背景图像随其余部分滚动而移动。
> - fixed：背景图像不移动。
> - inherit：从父元素继承。

```html
<html>
    <head>
        <style type="text/css">
            body {
                background-image: url("img/0004.jpg"); 
                background-repeat: no-repeat; 
                background-attachment: fixed; 
            }
        </style>
    </head>
    <body>
        <p>
            w3cschool
        </p>
    </body>
</html>
```

