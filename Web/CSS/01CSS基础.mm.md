# CSS基础

## CSS介绍

> CSS指**层叠样式表**（Cascading Style Sheets）
>
> 样式定义如何显示[HTML元素](../HTML/01基础.md)
>
> 样式通常存储在样式表中
>
> 把样式添加到HTML4.0中，是为了解决内容与表现分离的问题
>
> 外部样式表可以极大提高工作效率
>
> 外部样式表通常存储在CSS文件中
>
> 多个样式定义可层叠为一个

### 内联CSS

> 内联CSS也称为行内CSS/行级CSS，它直接在标签内部引用

```html
<p style="color:red; background-color:blue; ">
    Hi!I am a text!
</p>
```

<p style="color:red; background-color:blue; ">
    Hi!I am a text!
</p>

### 内部样式表

> 内部样式表定义在\<head>的\<style>元素中

```html
<html>
    <head>
        <!-- I will work on every paragraph! -->
        <style>
            p {color:white; background-color:gray; }
        </style>
    </head>
    <body>
        <p>
            I am the first paragraph.
        </p>
        <p>
            I am the second paragraph.
        </p>
    </body>
</html>
```

### 外部引用CSS

> CSS样式表存储在同一个后缀名为.css的拓展文件中。然后通过HTML标签\<link>在HTML页面的\<head>部分将CSS文件引入。

```html
<!-- HTMLpart -->
<head>
    <link rel="stylesheet" href="example.css" />
</head>
<body>
    <p>
        I am the first paragraph.
    </p>
    <p>
        I am the second paragraph.
    </p>
    <p>
        I am the third paragraph.
    </p>
</body>
```

```CSS
/* CSS part */
p {
    color:white;
    background-color:gray;
}
```

## CSS语法

> CSS是由浏览器解释的样式规则，然后应用于文档中相应的元素。
>
> 样式规则由三个部分：**选择器**，**属性**和**值**。`Selector { Property: Value; }`

### CSS注释

> CSS**注释**语法为：`/* 注释内容 */`

### CSS级联

> **级联**的顺序首先要根据**起源（origin）**将规则分类。
>
> 网页的最终外观是不同的样式结合的结果。
>
> 通过样式的三个主要来源形成一个级联：
>
> - 由页面作者创建的CSS样式
> - 浏览器的默认CSS样式
> - 浏览页买你的用户自定义的CSS样式
>
> 具体优先顺序：author > user > browser 。

### CSS继承

> **继承**是指属性在页面中流动的方式。除非另有定义，子元素通常会采用父元素的特征。

```html
<html>
    <head>
        <style>
            .father {
                color:red;
                font-size:24px;
            }
        </style>
    </head>
    <body>
        <div class="father">
            <div class="son">
                I am son.
            </div>
        </div>
    </body>
</html>
```

