# HTML5页面结构

> 通用的HTML5页面结构如下：

\![0002]\(img/0002.jpg "通用的HTML5页面结构")

![0002.jpg](https://i.loli.net/2021/01/25/ej4uFJ8lVKUOvNn.jpg "通用的HTML5页面结构")

### \<header>

> \<header>标签定义了文档的头部区域，适合在\<body>标签内部使用。

```html
<!DOCTYPE html>
<html>
    <head></head>
    <body>
        <header>
        	<h1>
                header 1
            </h1>
            <h3>
                header 3
            </h3>
        </header>
    </body>
</html>
```

### \<footer>

> \<footer>标签定义了文档或文档的一部分区域的页脚。

```html
<footer>
	<p>
        Powered by xingmo.
    </p>
</footer>
```

> 在典型情况下，\<footer>元素会包含文档创作者的姓名、文档的版权信息、使用条款的链接、联系信息等等。

### \<nav>

> \<nav>标签定义了导航链接部分。

```html
<nav>
	<a href="http://testftp002.tech:404">code代码仓库</a> |
    <a href="http://testftp002.tech">星痕墨迹</a> |
    <a href="http://testftp002.tech:6080">Xmail</a> |
    <a href="http://www.testftp002.site">Serv-U</a> |
</nav>
```

### \<artitle>

> \<artitle>标签定义了独立的内容。
>
> \<artitle>标签定义的内容本身必须是**有意义的且必须是独立于文档的其余部分**。
>
> \<artitle>潜在来源：
>
> - 论坛帖子
> - 博客文章
> - 新闻故事
> - 评论

```html
<artitle>
	<h1>
        artitle title
    </h1>
    <p>
        artitle details.
    </p>
</artitle>
```

### \<section>

> \<section>标签定义了文档的某个区域。比如**章节、头部、底部或者文档的其他区域**。

```html
<section>
	<h1>
        W3C
    </h1>
    <p>
        World Wide Web Consortium (W3C)... 
    </p>
</section>
```

### \<aside>

> \<aside>标签定义了\<artilte>标签外的内容。
>
> \<aside>的内容应该**与附近的内容相关**。

```html
<aside>
	<h4>
        Epcot Center
    </h4>
    <p>
        The Epcot Center is a theme park in Disney World, Florida.
    </p>
</aside>
```

> \<aside>的内容可用作文章的侧栏。