# JavaScript简介

### JavaScript基本特点

> - **轻量级**编程语言
> - **解释性**脚本语言
> - 可插入HTML页面
> - 可由所有现代浏览器执行

### JavaScript组成部分

> - ECMAScript：描述该语言的语法和基本对象
> - DOM（文档对象模型）：描述处理网页内容的方法和接口
> - BOM（浏览器对象模型）：描述与浏览器进行交互的方法和接口

### JavaScript用法

> `<script></script>`
>
> JavaScript可被放置在HTML页面的\<body>和\<head>部分中。

```html
<html>
    <head>
    </head>
    <body>
        <script>
        	alter("My First JavaScript!"); 
        </script>
    </body>
</html>
```

#### JavaScript输出

> - `document.write()`将内容写到HTML文档中
> - `window.alter()`弹出警告框
> - `innerHTML`写入到HTML元素
> - `console.log()`写入到浏览器的控制台

> 格式化文本（Formatting Text）

```html
<html>
    <head>
    </head>
    <body>
        <script>
        	document.write("<h1>Hello World!</h1>")
        </script>
    </body>
</html>
```

#### 外部JavaScript

> `<script src="example.js"></script>`

#### JavaScript注释

> 单行注释：`// JavaScript注释`
>
> 多行注释：`/* JavaScript注释 */`                                                                                                                                                                                                                                                                                            