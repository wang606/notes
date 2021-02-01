# HTML基础

## HTML标题标签

```html
<h1>这是一级标题</h1>

<h2>这是二级标题</h2>

<h3>这是三级标题</h3>

<h4>这是四级标题</h4>

<h5>这是五级标题</h5>

<h6>这是六级标题</h6>
```

## HTML水平线

```html
<hr/>
```

## HTML注释

```html
<!-- 注释内容 -->
```

## HTML段落

```html
<p>段落</p>
```

> 浏览器会自动在段落前后添加空行！

## HTML拆行

> 在不产生一个新段落的情况下进行换行。

```html
<br/>
```

## HTML格式化标签

> \<b>粗体\</b>
>
> \<i>斜体\</i>
>
> \<s>删除线\</s>
>
> \<u>下划线\</u>
>
> \<sub>定义下标字\</sub>
>
> \<sup>定义上标字\</sup>
>
> \<small>定义小号字\</small>

```html
<b>粗体</b>

<i>斜体</i>

<s>删除线</s>

<u>下划线</u>

<sub>定义下标字</sub>

<sup>定义上标字</sup>

<small>定义小号字</small>
```

## HTML链接

> 使用href属性来描述链接的目标地址。

```html
<a href="http://127.0.0.1">Serv-U</a>
```

> 使用target属性规定在何处打开链接文档。
>
> ​	_blank:在新窗口中打开被链接文档。
>
> ​	_self:默认。在相同的框架中打开被链接文档。
>
> ​	_parent:在父框架集中打开被链接文档。
>
> ​	_top:在整个窗口中打开被链接文档。
>
> ​	framename:在指定的框架中打开被链接文档。

```html
<a href="http://127.0.0.1" target="_blank">Serv-U</a>
<a href="http://127.0.0.1" target="_self">Serv-U</a>
<a href="http://127.0.0.1" target="_parent">Serv-U</a>
<a href="http://127.0.0.1" target="_top">Serv-U</a>
<a href="http://127.0.0.1" target="framename">Serv-U</a>
```

> 使用title属性设置鼠标放在链接上时显示的文字。

```html
 <a href="http://127.0.0.1" target="_blank" title="code代码仓库">Serv-U</a>
```

## HTML头部

> \<head>元素包含了所有的头部标签元素。
>
> 在\<head>元素中可以插入脚本（scripts），样式文件（CSS），及各种meta信息。
>
> ​	\<head>定义了文档的信息。
>
> ​	\<titile>定义了文档的标题。
>
> ​	\<base>定义了页面链接标签的默认链接地址。
>
> ​	\<link>定义了一个文档和外部资源之间的关系。
>
> ​	\<meta>定义了HTML文档中的元数据。可以为搜索引擎定义关键词；为网页定义描述内容；定义网页作者；或其他Web服务。
>
> ​	\<script>定义了客户端的脚本文档。
>
> ​	\<noscript>定义在脚本未被执行是的代替内容（文本）。
>
> ​	\<style>定义了HTML文档的样式文件。

```html
<html>
	<head>
		<title>浏览器工具栏中的标题</title>
         <!-- <link>标签用于链接到CSS样式表 -->
         <link rel="stylesheet" type="text/css" href="mystyle.css">
         <!-- <link>标签设置网页图标 -->
         <link rel="shortcut icon" href="picture_url">
         <!-- <meta>标签为搜索引擎定义关键词 -->
		<meta name="keywords" content="HTML";>
         <!-- <meta>标签为网页定义描述内容 -->
		<meta name="description" content="HTML学习";>
         <!-- <meta>标签定义网页作者 -->
		<meta name="author" content="wang tsinghua";>
         <!-- <meta>标签设置每30秒刷新当前页面 -->
		<meta http-equiv="refresh" content="30";>
         <!-- <meta>标签定义字符集 -->
		<meta charset=utf-8;>
         <style type="text/css">
             body {background-color:yellow}
             p {color:blue}
         </style>
    </head>
</html>
```

## HTML CSS

> ​	CSS(层叠样式表或级联样式表 Cascading Style Sheets)是用于渲染HTML元素标签的样式。
>
> ​	CSS可以通过以下方式添加到HTML中：
>
> - 内联样式：在HTML元素中使用\<style>属性。
> - 内部样式表：在HTML文档头部\<head>区域使用\<style>元素来包含CSS。
> - 外部引用：使用外部CSS文件。

```html
<!-- 内联样式 -->
<h1 style="font-family:arial; text-align:center; ">
    学习HTML
</h1>
<p style="font-family:arial; color:red; font-size:20px; ">
    CSS内联样式
</p>
```

```html
<!-- 内部样式表 -->
<head>
<style type="text.css">
    h1 {color:red;}
    p {color:blue;}
</style>
</head>
```

```html
<!-- 外部样式表 -->
<head>
    <link rel="stylesheet" type="text/css" href="../res/css/基础.css">
</head>
```

## HTML图像

> \<img src="图像_url"> 
>
> alt属性用来为图像定义一串预备的可替代的文本。
>
> width、height属性用于指定设置图像的宽度与高度。单位为px（像素【默认】）或%（百分比）。

```html
<img src="../res/img/p001.png" alt="射击游戏" width="800" height="400">
```

## HTML列表

> 无序列表
>
> \<ul>:unordered lists
>
> \<li>:list item

```html
<ul>
	<li>apple</li>
    <li>banana</li>
    <li>pineapple</li>
</ul>
```

> 有序列表
>
> \<ol>:ordered lists
>
> \<li>:list item

```html
<ol>
	<li>apple</li>
    <li>banana</li>
    <li>pineapple</li>
</ol>
```

> 自定义列表
>
> \<dl>:definition lists(自定义列表)
>
> \<dt>:definition term(自定义列表组)
>
> \<dd>:definition description(自定义列表描述)

```html
<dl>
    <dt>apple</dt>
    	<dd>big and red</dd>
    <dt>banana</dt>
    	<dd>smell and sweet</dd>
</dl>
```

## HTML区块

> HTML块级元素（在浏览器中显示时，通常会以新行来开始和结束，另起一行，如：\<div>,\<h1>,\<p>,\<ul>,\<table>等元素。）
>
> HTML内联元素（在浏览器中显示时，通常不会以新行来开始和结束，如：\<span>,\<a>,\<img>,\<b>,\<td>等元素。）

> \<div>元素是块级元素，可用于组合其他HTML元素的容器。如果与CSS一同使用，\<div>元素可用于对大的内容块设置样式属性。

```html
<div style="color:#FF0000">
    <h1>
        div中的元素标题
    </h1>
    <p>
        div中的文本
    </p>
</div>
```

> \<span>元素是内联元素，可用作文本的容器。如果与CSS一同使用，\<span>元素可用于对部分的文本设置样式属性。

```html
<p>我的哥哥有<span style="color:#0000FF; font-weight:bold">蓝色</span>的球鞋，我的姐姐有<span style="color:#FF0000; font-weight:bold">红色</span>的球鞋。</p>
```

## HTML框架

> \<iframe>标签规定一个内联框架。一个内联框架被用来在当前HTML文档中嵌入另一个文档。
>
> width、height属性用于指定设置图像的宽度与高度。单位为px（像素【默认】）或%（百分比）。
>
> frameborder属性用于定义是否显示边框。（1【默认】：开启边框；0：移除边框。）

```html
<iframe src="https://www.w3cschool.cn" width="300" height="300" frameborder="0">
</iframe>
```

## HTML颜色

> \#000000 ~ \#FFFFFF

## HTML脚本

> 向HTML添加脚本，使HTML页面具有更强的动态性和交互性。
>
> \<script>:定义了客户端脚本。
>
> \<noscript>:定义了不支持脚本浏览器输出的文本。

```html
<script>
document.write("Hello world!");
</script>
<nosript>
抱歉，您的浏览器不支持JavaScript！
</nosript>
```

## HTML字符实体

> | 显示结果 | 描述        | 实体名称  | 实体编号 |
> | -------- | ----------- | --------- | -------- |
> |          | 空格        | \&nbsp;   | \&#160;  |
> | <        | 小于号      | \&lt;     | \&#60;   |
> | >        | 大于号      | \&gt;     | \&#62;   |
> | &        | 和号        | \&amp;    | \&#38;   |
> | "        | 引号        | \&quot;   | \&#34;   |
> | '        | 撇号        | \&apos;   | \&#39;   |
> | &cent;   | 分          | \&cent;   | \&#162;  |
> | &pound;  | 镑          | \&pound;  | \&#163;  |
> | ￥       | 人民币/日元 | \&yen;    | \&#165;  |
> | &euro;   | 欧元        | \&euro;   | \&#8364; |
> | &sect;   | 小节        | \&sect;   | \&#167;  |
> | &copy;   | 版权        | \&copy;   | \&#169;  |
> | &reg;    | 注册商标    | \&reg;    | \&#174;  |
> | &trade;  | 商标        | \&trade;  | \&#8482; |
> | &divide; | 除号        | \&divide; | \&#247;  |
# HTML表格

### HTML表格标签

> \<table>
>
> \<tr>:table row（一行）
>
> \<th>:table header cell（表头）
>
> \<td>:table data cell（单元格）

```html
<table border='1'>
    <tr>
    	<td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
        <td>row 1, cell 3</td>
    </tr>
    <tr>
    	<td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
        <td>row 2, cell 3</td>
    </tr>
</table>
```

> \<caption>:定义表格的标题。
>
> \<colgroup>:定义表格列的组。
>
> \<col>:定义表格列的属性。
>
> \<thead>:定义表格的页眉。
>
> \<tbody>:定义表格的主体。
>
> \<tfoot>:定义表格的页脚。

### HTML合并单元格

> rowspan属性定义单元格横跨的行数。
>
> colspan属性定义单元格横跨的列数。

```html
<table border="1">
    <tr>
    	<td>Name:</td>
        <td>wang tsinghua</td>
    </tr>
    <tr>
    	<td rowspan="2">mail:</td>
        <td>wang__qing__hua@163.com</td>
    </tr>
    <tr>
    	<td>3372938775@qq.com</td>
    </tr>
</table>
```

```html
<table border="1">
    <tr>
    	<th>Month</th>
    	<th>Savings</th>
    </tr>
    <tr>
    	<td>January</td>
        <td>$500</td>
    </tr>
    <tr>
    	<td>February</td>
        <td>$480</td>
    </tr>
    <tr>
    	<td colspan="2">Sum:$980</td>
    </tr>
</table>
```

# HTML表单

> 表单是一个包含表单元素的区域。
>
> 表单元素允许用户在表单中插入内容，如：文本框、下拉列表、单选框、复选框等等。
>
> HTML表单用于收集不同类型的用户输入。

### HTML\<form>标签

#### action属性：

> 规定当提交表单时，向何处发送表单数据。

```html
<form action="URL">
```

> URL:
>
> - 绝对URL - 指向另一个网站（比如action="https://www.w3cschool.cn/index.html"）
> - 相对URL - 指向网站内的一个文件（如action="index.html"）

#### method属性：

> 规定如何发送表单数据。

```html
<form method="get | post">
```

> get:以查询字符串形式提交，在地址栏中能看到，长度有限制，不安全。
>
> post:以表单数据组形式提交，在地址栏中看不到，长度无限制，安全。

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <titile>use "get" to submit a form</titile>
    </head>
    <body>
        <form action="get_method.php" method="get" target="_blank">
            user: <input type="text" name="user"><br/>
            password: <input type="password" name="password"><br/>
            <input type="submit" value="sign in">
        </form>
        <p>
            click the "sign in" button,the statics in inputing area will be sent to get_method.php!
        </p>
    </body>
</html>
```

#### enctype属性：

> 规定在将表单数据发送到服务器之前如何对其进行编码。

> 注意：只有method="post"时才使用enctype属性。
>
> enctype属性值有：
>
> - application/x-www-form-urlencoded:【默认】在发送前对所有字符进行编码（将空格转换为"+"符号，特殊字符转换为ASCII HEX值）。
> - multipart/form-data:不对字符编码。当使用有文件上传控件的表单时，该值是必须的。

### HTML表单输入元素

> 输入标签\<input>
>
> 输入类型type:
>
> - 文本框（text）
> - 密码字段（password）
> - 单选按钮（radio）
> - 复选框（checkbox）
> - 提交按钮（submit）

#### 文本框

```html
<form>
    Username: <input type="text" name="username">
</form>
```

#### 密码字段

```html
<form>
    Password: <input type="password" name="pwd">
</form>
```

#### 单选按钮

```html
<form>
    Sex:<br/>
    <input type="radio" name="sex" value="male">Male<br/>
    <input type="radio" name="sex" value="female">Female<br/>
</form>
```

#### 复选框

```html
<form>
    check what you want:<br/>
    <input type="checkbox" name="Fruit" value="apple">Apple<br/>
    <input type="checkbox" name="Fruit" value="banana">Banana<br/>
</form>
```

#### 提交按钮

```html
<form action="html_form_action.php" method="post" name="myForm">
    invation: <input type="password" name="invation">
    <input type="submit" value="Corfirm">
</form>
```

### HTML特殊表单元素

#### 下拉列表

> \<select>标签定义了下拉选项列表。
>
> \<select>中的\<option>标签定义列表中的可用选项。

```html
<select>
    <option value="1">Apple</option>
    <option value="2">Banana</option>
    <option value="3">Orange</option>
</select>
```

#### 文本域

> \<textarea>标签定义文本域。
>
> cols、rows属性分别规定了文本区域内可见的宽度和高度。

```html
<textarea rows="3" cols="20">input something</textarea>
```

### HTML其他表单元素

#### \<label>

> \<label>标签定义了\<input>元素的标签，一般为输入标题。

```html
<form action="label_form.php">
    <label for="1">Male</label>
    <input type="radio" name="sex" id="1" value="male"><br/>
    <label for="2">Female</label>
    <input type="radio" name="sex" id="2" value="female"><br/>
    <input type="submit" value="I am a human.">
</form>
```

> 点击\<label>标签，浏览器会自动将焦点转移到和标签相关的表单控件上。

#### \<button>

> \<button>标签定义一个按钮。
>
> 在\<button>元素内部可以放置内容，如文本或图像。
>
> \<button>type属性值有：
>
> - submit：【默认】提交按钮
> - button：可点击按钮
> - reset：重置按钮

```html
<button type="button">a magic button!</button>
```

#### \<fieldset>

> \<fieldset>标签定义了一组相关的表单元素，并使用外框包含起来。
>
> \<legend>标签定义了\<fieldset>元素的标题。

```html
<form>
    <fieldset>
        <legend>
            Author: 
        </legend>
        Name: <input type="text"><br/><br/>
        Telephone: <input type="text"><br/><br/>
        Email: <input type="text">
    </fieldset>
</form>
```

# HTML5

> HTML5的设计目的是为了在移动设备上支持多媒体。
>
> HTML5还引进了新的功能，可以真正改变用户与文档的交互方式。

> 在编写HTML5文档时，\<!DOCTYPE html>声明必须位于HTML5文档中的第一行：

````html
<!DOCTYPE html>
````

> 字符编码（字符集）声明也被简化：

```html
<mata charset="UTF-8" />
```

> HTML5中默认字符集编码是UTF-8。
>
> 对于中文网也需要使用\<meta charset="utf-8" />声明编码。

> HTML5的新特性：
>
> - 用于绘画的canvas元素
> - 用于媒体回放的video和audio元素
> - 对本地离线储存的更好的支持localStorage、sessionStorage
> - 新的特殊内容元素，如article、footer、header、nav、section
> - 新的表单控件，如calendar、date、time、email、url、search
> - 



# HTML5内容模型

> HTML5中标记元素根据内容模型的不同被分为7大类：
>
> - 内联（Embedded）
> - 流（Flow）
> - 标题（Heading）
> - 交互（Interactive）
> - 元数据（Metadata）
> - 短语（Phrasing）
> - 区段（Sectioning）

### 元数据（Metadata）

> 通常出现在页面的head中，设置页面其他部分的表现和行为。
>
> 元素：\<base>，\<link>，\<mata>，\<noscript>，\<script>，\<style>，\<title>。

### 内联（Embedded）

> 在文档中添加其他类型的内容。
>
> 元素：\<audio>，\<video>，\<canvas>，\<iframe>，\<img>，\<math>，\<object>，\<svg>。

### 交互（Interactive）

> 与用户交互的内容。
>
> 元素：\<a>，\<audio>，\<video>，\<button>，\<details>，\<embed>，\<iframe>，\<img>，\<input>，\<label>，\<object>，\<select>，\<textarea>。

### 标题（Heading）

> 定义段落标题。
>
> 元素：\<h1-6>，\<hgroup>。

### 短语（Phrasing）

> 文本和文本标记元素。
>
> 元素：\<img>，\<span>，\<b>，\<label>，\<br/>，\<small>，\<sub>等等。

### 流（Flow）

> 包含在文档正常流中的大多数HTML5元素。

### 区段（Sectioning）

> 定义标题，内容，导航和页脚的范围。
>
> 元素：\<article>，\<aside>，\<nav>，\<section>。

\![0001]\(img\0001.jpg "HTML5内容模型")

![0001.jpg](https://i.loli.net/2021/01/25/iYpjXUKIFHnoPZA.jpg "HTML5内容模型")



# HTML5元素分类

> HTML5的元素按优先等级定义为**结构性元素**、**级块性元素**、**行内语义性元素**、**交互性元素**四大类。

## 结构性元素

> 结构性元素主要负责Web的上下文结构的定义，确保HTML文档的完整性。

### section

> 在Web页面应用中，该元素也可以用与区域的章节表述。

```html
<section>
	<h1>
        math_
    </h1>
    <p>
        It is used for math!
    </p>
</section>
<h1>
    math_
</h1>
<p>
	It is used for math!
</p>
```

### header

> 页面主题上的头部。

```html
<header>
	<h1>
        Internet Explorer
    </h1>
    <p>
        <time pubdate datetime="2021-01-25"></time>
    </p>
</header>
```

### footer

> 页面的底部（页脚）。

```html
<footer>
	<p>
        powered by xingmo.
    </p>
    <p>
        <time pubdate datetime="2021-01-25"></time>
    </p>
</footer>
```

### nav

> nav是专门用于菜单导航。链接导航的元素，是navigator的缩写。

```html
<nav>
	<a href="http://testftp002.tech:404">code代码仓库</a> |
    <a href="http://testftp002.tech">星痕墨迹</a> |
    <a href="http://testftp002.tech:6080">Xmail</a> |
    <a href="http://www.testftp002.site">Serv-U</a> |
</nav>
```

### article

> 用于表示一篇文章的主体部分，一般为文字集中显示的区域。

```html
<article>
	<h1>
        Internet Explorer 9
    </h1>
    <p>
        Windows Internet Explorer 9 is published in March 14th 2011.
    </p>
</article>
```

## 级块性元素

> 级块性元素主要完成Web页面区域的划分，确保内容的有效隔离。

### aside

> 用于表达注记、贴士、侧栏、摘要、插入的引用等作为补充主体的内容。

```html
<p>
    My family and I visited The Epcot Center this summer.
</p>
<aside>
	<h4>
        Epcot Center
    </h4>
    <p>
        The Epoct Center is a theme park in Disney World,Florida.
    </p>
</aside>
```

### figure

> 对多个元素进行组合并展示，通常与\<figcaption>联合使用。

```html
<figure>
	<img src="https://i.loli.net/2021/01/25/iYpjXUKIFHnoPZA.jpg" alt="The Pulpit Rock" width="304" height="228">
    <figcaption>Fig1. - A view of the pulpit rock in Norway.</figcaption>
</figure>
```

### code

> 表示一段代码块。

```html
<code>
	<h4>
        Epcot Center
    </h4>
    <p>
        The Epoct Center is a theme park in Disney World,Florida.
    </p>
</code>
<h4>
    Epcot Center
</h4>
<p>
    The Epoct Center is a theme park in Disney World,Florida.
</p>
```

### dialog

> 用于表达人与人之间的对话，该元素还包括\<dt>和\<dd>这两个组合元素。\<dt>用于表示说话者，而\<dd>用于表示说话者的内容。

```html
<dialog open>
	<dt>note:</dt>
    <dd>no zuo will die</dd>
</dialog>
```

## 行内语义性元素

> 行内语义性元素主要完成Web页面具体内容的引用和表述，是丰富内容展示的基础。

### meter

> 表示特定范围内的数值，可用于工资、数量、百分比等。

```html
<meter value="2" min="0" max="10">2 out of 10</meter><br/>
<meter value="0.6">60%</meter>
```

### time

> 表示时间值。

```html
<p>
    We must go to school at <time>8:00</time> everyday.
</p>
<p>
    I have a class in <time datetime="2021-02-14">Valentine's Day</time>.
</p>
```

### mark

> 定义带有记号的文本。

```html
<p>
    Do not forget to buy <mark>milk</mark> today.
</p>
```

### progress

> 用来表示进度条，可通过对其max、min、step等属性进行控制，完成对进度的表示和监视。

```html
<progress value="22" max="100"></progress>
```

### video

> 视频元素，用于支持的实现视频（含视频流）文件的直接播放，支持缓冲预载和多种视频格式，如MPEG-4、OggV和WebM等。

```html
<video width="320" height="240" controls>
	<source src="https://www.w3cschool.cn/statics/demosource/mov_bbb.mp4" type="video/mp4">
    <source src="https://www.w3cschool.cn/statics/demosource/mov_bbb.ogg" type="video/ogg">
    your browser doesn't support video!
</video>
<video width="512" height="389" controls>
	<source src="video/车厢桥.avi" type="video/avi">
    Vedio in HTML5 doesn't support avi!
</video>
```

### audio

> 音频元素，用于支持和实现音频（含音频流）文件的直接播放，支持缓冲预载和多种音频媒体格式。

```html
<audio controls>
	<source src="https://www/w3cschool.cn/statics/demosource/horse.mp3" type="audio/ogg">
    <source src="https://www/w3cschool.cn/statics/demosource/horse.ogg" type="audio/mpeg">
    your browser doesn't support audio!
</audio>
```

## 交互性元素

> 交互性元素主要用于功能性的内容表达，会有一定的内容和数据的关联，是各种事件的基础。

### details

> 用来表示一段具体的内容，但是内容默认可能不显示，通过某种手段（如单击）与\<kegend>交互才会显示出来。

```html
<details>
	<summary>W3Cschool</summary>
    <p>
         - by W3Cschool Data. ALL Rights Reserved.
    </p>
    <p>
        All content and graphics on this web site are the property of the company W3Cschool Data.
    </p>
</details>
```

### detalist

> 定义选项列表。与input元素配合使用可定义input可能的值。

```html
<input list="browsers">
<datalist id="browsers">
	<option value="Internet Explorer"></option>
    <option value="Firefox"></option>
    <option value="Chrome"></option>
    <option value="Opera"></option>
    <option value="Safari"></option>
</datalist>
```

### menu

> 主要用于交互菜单。

```html
<menu type="toolbar">
	<li>
    	<menu label="File">
        	<button type="button" onclick="file_new()">
                new
            </button>
            <button type="button" onclick="file_open()">
                open
            </button>
            <button type="button" onclick="file_save()">
                save
            </button>
        </menu>
    </li>
    <li>
    	<menu label="Edit">
        	<button type="button" onclick="edit_cut()">
                cut
            </button>
            <button type="button" onclick="edit_copy()">
                copy
            </button>
            <button type="button" onclick="edit_paste()">
                paste
            </button>
        </menu>
    </li>
</menu>
```

### command

> 用来处理命令按钮。

```html
<menu>
    <command type="command" label="Save" onclick="save()">Save</command>
</menu>
```



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





# HTML5 Audio元素

> \<audio>标签定义声音，比如**音乐或其他音频流**。目前，\<audio>元素支持3种文件格式：MP3、Wav、Ogg。

```html
<audio controls>
	<source src="https://www/w3cschool.cn/statics/demosource/horse.mp3" type="audio/ogg">
    <source src="https://www/w3cschool.cn/statics/demosource/horse.ogg" type="audio/mpeg">
    your browser doesn't support audio!
</audio>
```

> \<source>标签用来定义多种媒体资源，\<control>属性供添加播放、暂停和音量控件。
>
> \<audio>元素允许使用多个\<source>以链接不同的音频文件，浏览器将使用第一个支持的音频文件。
>
> \<audio>与\</audio>之间的文字将在不支持\<audio>标签的浏览器上显示。

> src属性规定音频文件的URL。
>
> autoplay属性让音频在就绪后马上播放。
>
> loop属性让音频结束时重新开始播放。



# HTML5 Video元素

> \<video>标签定义视频，比如**电影片段或其他视频流**。目前，\<video>元素支持三种是视频格式：MP4、WebM、Ogg。

```html
<video width="320" height="240" controls>
	<source src="https://www.w3cschool.cn/statics/demosource/mov_bbb.mp4" type="video/mp4">
    <source src="https://www.w3cschool.cn/statics/demosource/mov_bbb.ogg" type="video/ogg">
    your browser doesn't support video!
</video>
<video width="512" height="389" controls>
	<source src="video/车厢桥.avi" type="video/avi">
    Vedio in HTML5 doesn't support avi!
</video>
```

> \<source>标签用来定义多种媒体资源，\<control>属性供添加播放、暂停和音量控件。
>
> \<video>元素允许使用多个\<source>以链接不同的视频文件，浏览器将使用第一个支持的视频文件。
>
> \<video>与\</video>之间的文字将在不支持\<video>标签的浏览器上显示。

> src属性规定视频文件的URL。
>
> width、height属性控制视频的尺寸。
>
> autoplay属性让视频在就绪后马上播放。
>
> loop属性让视频结束时重新开始播放。





# HTML5表单

### placeholder属性

> placeholder属性在\<input>和\<textarea>元素上提供提示，描述输入域所期待的值。提示在用户输入之前会显示在输入域上。

```html
<form>
    <input type="text" name="firstname" placeholder="First name"><br/>
    <input type="text" name="lastname" placeholder="Last name"><br/>
    <input type="submit" value="Confirm">
</form> 
```

### autofocus属性

> autofocus属性规定在页面添加加载时，域自动地获得焦点。

```html
<form>
    <input type="text" name="firstname" placeholder="First name autofocus"><br/>
    <input type="text" name="lastname" placeholder="Last name"><br/>
    <input type="submit" value="Confirm">
</form> 
```

### required属性

> required属性规定必须在提交之前填写输入域（不能为空）。

```html
<form autocomplete="off">
    Username: <input type="text" name="username" required>
    <input type="submit">
</form>
```

> autocomplete属性规定form或input域应该拥有自动完成功能。当用户在自动完成域中开始输入时，浏览器应该在该域或中显示填写的选项。

### search类型

> search类型可用于创建搜索框。

```html
<input type="search" name="searchitem">
```

### \<datalist>

> \<datalist>元素规定输入域的选项列表。

```html
<input list="browsers">
<datalist id="browsers">
	<option value="Internet Explorer"></option>
    <option value="Firefox"></option>
    <option value="Chrome"></option>
    <option value="Opera"></option>
    <option value="Safari"></option>
</datalist>
```

### 更多的输入类型

> email、tel、url、date、time等。

```html
<form>
    <input type="email" name="email" placeholder="example@example.com"><br/>
    <input type="tel" name="tel" placeholder="000.000.0000"><br/>
    <input type="url" name="homepage" placeholder="example.com">
</form>
```




# HTML5SVG

> SVG指可伸缩矢量图形（Scalable Vector Graphics）
>
> SVG用于定义用于网络的基于矢量的图形
>
> SVG使用XML格式定义图形
>
> SVG图像在放大或改变尺寸的情况下其图形质量不会有损失
>
> SVG是万维网联盟的标准

### SVG圆形(circle)

```html
<svg width="1000" height="1000">
	<circle cx="100" cy="50" r="40" fill="blue" />
</svg>
```

> cx、cy属性分别定义圆心的x、y坐标，默认值为0
>
> r属性定义圆的半径

### SVG矩形(rect)

```html
<svg width="1000" height="1000">
	<rect width="400" height="200" x="20" y="20" fill="red" />
</svg>
```

### SVG直线(line)

```html
<svg width="500" height="500">
	<line x1="20" y1="20" x2="300" y2="200" style="stroke:#000000; stroke-linecap:round; stroke-width:20" />
</svg>
```

### SVG曲线(polyline)

```html
<svg width="2000" height="500">
	<polyline style="stroke-linejoin:miter; stroke:black; stroke-width:12; fill:none;" points="100 100, 150 150, 200 100" />
</svg>
```

> points属性：每两个数字为一组，定义一个坐标点位置。
>
> stroke属性：定义图形边框的颜色。
>
> stroke-width属性：定义图形边框的宽度。
>
> stroke-linecap属性：定义端点，默认为方形，round为圆形。

### SVG椭圆(ellipse)

```html
<svg width="500" height="250">
	<ellipse cx="200" cy="100" rx="150" ry="70" style="fill:#808000; " />
</svg>
```

### SVG多边形(polygon)

```html
<svg width="1000" height="1000">
	<polygon points="100 100, 200 200, 300 0" style="fill:#800080; stroke:#000000; " />
</svg>
```



# HTML5SVG动画&路径

## SVG动画

> SVG动画可以使用\<animate>元素创建。

```html
<svg width="1000" height="250">
	<rect width="150" height="150" fill="orange">
    	<animate attributeName="x" from="0" to="300" dur="3s" fill="freeze" repeatCount="2" />
    </rect>
</svg>
```

> attributeName:指定哪个属性需要产生动画效果。
>
> from:指定属性的起始值。
>
> to:指定属性的结束值。
>
> dur:指定动画运行的时间（持续时间）。
>
> fill="freeze | remove":指定动画播放完毕后是停留在播放的终点（freeze）还是回到起始位置（remove）。
>
> repeatCount:指定动画的重复播放次数，indefinite为无数次。

## SVG路径

> \<path>元素用于定义一个路径。
>
> 下面的命令可用于路径数据：【大写标识绝对定位，小写表示相对定位】
>
> - M/m = moveto
> - L/l = lineto
> - H/h = horizontal lineto
> - V/v = vertical lineto
> - C/c = curveto
> - S/s = smooth curveto
> - Q/q = quadratic Bézier curve
> - T/t = smooh quadratic Bézier curveto
> - A/a = elliptical Arc
> - Z/z = closepath

```html
<svg width="500" height="500">
	<path d="M150 0 L75 200 L225 200 Z" />
</svg>
```



# HTML5Canvas

> \<canvas>标签只是图形容器，需配合脚本来绘制图形。
>
> \<canvas>标签通常需要指定一个id属性（脚本中经常引用），width和height属性定义的画布大小。
>
> getContext()方法可返回一个对象，该对象提供用于在画布上绘画的方法和属性。
>
> 我们可通过多种方法使用Canvas绘制路径、盒、圆、字符以及添加图像。

```html
<canvas id="canvas01" width="200" height="100"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    ctx.fillStyle="#808000";//填充矩形的颜色
    ctx.fillRect(0, 0, 150, 75);//绘制一个矩形，fillRect(x, y, width, height)
</script>
```

### canvas路径

> moveTo(x, y)定义线条开始坐标。
>
> lineTo(x, y)定义线条结束坐标。

```html
<canvas id="canvas01" width="200" height="100"></canvas>
<script>
	var c=document.getElementById("canvas01");
	var ctx=c.getContext("2d");
	ctx.moveTo(0, 0);
	ctx.lineTo(200, 100);
	ctx.stroke();
</script>
```

### canvas圆形/扇形

> arc(x, y, r, start, stop)

```html
<canvas id="canvas01" width="200" height="100"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    ctx.beginPath();
    ctx.arc(95, 50, 40, 0, 2*Math.PI);
    ctx.stroke();
</script>
```

### canvas文本

> font定义字体。
>
> fillText(text, x, y)在canvas上绘制实心的文本。
>
> strokeText(text x, y)在canvas上绘制空心的文本。

```html
<canvas id="canvas01" width="200" height="100"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    ctx.font="30px Arial";
    ctx.fillText("hello world!", 10, 50);
    ctx.strokeText("hello world!", 10, 100);
</script>
```

### canvas渐变

> 渐变可以填充在矩形，圆形，线条，文本等等，各种形状可以定义自己不同的颜色。
>
> createLinearGradient(x, y, x1, y1)创建线条渐变。
>
> createRadialGradient(x, y, r, x1, y1, r1)创建一个径向/圆渐变。
>
> addColorStop()方法指定颜色停止，参数使用坐标描述，可以是0至1。
>
> 使用渐变，先设置fillStyle或strokeStyle的值为gradient，然后绘制形状。

```html
<canvas id="canvas01" width="200" height="100"></canvas>
<script>
	var c1=document.getElementById("canvas01");
    var ctx1=c1.getContext("2d");
    var c2=document.getElementById("canvas01");
    var ctx2=c2.getContext("2d");
    //create gradients
    var grd1=ctx1.createLinearGradient(0, 0, 200, 0);
    grd1.addColorStop(0, "red");
    grd1.addColorStop(1, "white");
    var grd2=ctx2.createRadialGradient(75, 50, 5, 90, 60, 100);
    grd2.addCOlorStop(0, "bule");
    grd2.addColorStop(1, "#00FF00");
    //fill the gradients
    ctx1.fillStyle=grd1;
    ctx1.fillRect(10, 10, 150, 80);
    ctx2.fillStyle=grd2;
    ctx2.fillRect(10, 10, 150, 80);
</script>
```

### canvas图像

> drawImage(img, x, y)可将一幅图像放置到画布上。

```html
<canvas id="canvas01" width="200" height="100"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    var img=document.getElementById("myimg");
    ctx.drawImage(img, 10, 10);
</script>
```

\![0003]\(../img/0003.jpg "SVG与Canvas的区别")

![0003](https://i.loli.net/2021/01/25/DQC21iHf3eNV7wd.jpg "SVG与Canvas的区别")



# HTML5Canvas转换

### 平移translate()

> translate(x, y)方法用于移动Canvas。

```html
<canvas id="canvas01" width="200" height="400"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    ctx.font="bold 20px Arial";
    ctx.textAlign="Hello world!";
    ctx.fillText("Hello world!", 20, 40);
    ctx.translate(100, 150);
    ctx.fillText("after translate", 20, 40);
</script>
```

### 旋转rotate()

> rotate()用于旋转HTML5画布。

```html
<canvas id="canvas01" width="200" height="400"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    ctx.fillStyle="#008080";
    ctx.fillRect(10, 10, 100, 100);
    //rotate 25 degree.
    ctx.rotate(Math.PI / 180 * 25);
    ctx.fillStyle="#800080";
    ctx.fillRect(10, 10, 100, 100);
</script>
```

### 缩放scale()

> scale(x_times, y_times)缩放当前绘图，使x方向变为x_times倍，使y方向变为y_times倍。

```html
<canvas id="canvas01" width="300" height="400"></canvas>
<script>
	var c=document.getElementById("canvas01");
    var ctx=c.getContext("2d");
    ctx.strokeRect(5, 5, 25, 15);
    ctx.scale(2, 2);
    ctx.strokeRect(5, 5, 25, 15);
    ctx.scale(2, 2);
    ctx.strokeRect(5, 5, 25, 15);
    ctx.scale(2, 2);
    ctx.strokeRect(5, 5, 25, 15);
</script>
```



# HTML5Web存储

> 在HTML5之前，本地存储使用的是cookie。
>
> Web存储的优势：
>
> - 更加安全
> - 更加快速
> - 可以存储大量的数据
> - 每个服务器请求都不会发送存储的数据
>
> 数据以 键/值 对存在，Web网页的数据只允许该网页访问使用。

> Web储存对象有两种类型：
>
> - localStorage：存储的数据没有时间限制。
> - sessionStorage：针对一个session进行数据存储。当用户关闭浏览器窗口后，数据会被删除。

> Web存储使用的API：
>
> - 保存数据：
>
>   localStorage.setItem(key, value);
>
> - 读取数据：
>
>   localStorage.getItem(key);
>
> - 删除单个数据：
>
>   localStorage.removeItem(key);
>
> - 清除所有数据：
>
>   localStorage.clear();
>
> - 得到某个索引的key:
>
>   localStorage.key(index);



# HTML5地理定位

> Geolocation API用于获取用户的地理位置，其主要方法是getCurrentPosition。

```html
<div id="demo"></div>
<script>
	var x=document.getElementById("demo");
    function getLocation(){
        if (navigator.geolocation){
            navigaor.geolocation.getCurrentPosition(showPosition);
        }
        else{
            x.innerHTML="your browser doesn't support Geolocation!";
        }
    }
    function showPosition(position){
        x.innerHTML="latitude: " + position.coords.latitude + "<br/>longitude: " + position.coords.longitude;
    }
</script>
```

### 百度API

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>baiduAPI</title>
		<!-- 引入百度API，ak是密钥，可以自己申请。 -->
        <script type="text/javascript" src="https://api.map.baidu.com/api?v=2.0&ak=7a6QKaIilZftIMmKGAFLG7QT1GLfIncg"></script>
    </head>
    <body> 
        <input type="button" onclick="getLocation()" value="定位" />
        <div id="position"></div>
        <script type="text/javascript">
        	var x=document.getElementById("position");
            function getLocation(){
                //创建百度API位置实例，代替navigator.geolaocation
                var geolocation=new BMap.Geolocation();
                geolocation.getCurrentPosition(function(e) {
                    if (this.getStatus() == BMAP_STATUS_SUCCESS){
                        x.innerHTML="纬度：" + e.point.lat + "<br/>经度：" + e.point.lng;
                    }
                    else {
                        x.innerHTML="failed" + this.getStatus();
                    }
                });
            }
        </script>
    </body>
</html>
```




# HTML5拖放

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>W3Cschool</title>
        <style type="text/css">
        	#div01 {width:350px; height:200px; padding:10px; border:1px solid #aaaaaa; }
        </style>
        <script>
        	function allowDrop(ev) {
                ev.preventDefault();
            }
            function drag(ev) {
                ev.dataTransfer.setData("Text", ev.target.id);
            }
            function drop(ev) {
                ev.preventDefault();
                var data=ev.dataTransfer.getData("Text");
                ev.target.appendChild(document.getElementById(data));
            }
        </script>
    </head>
    <body>
        <p>
            拖动图片到矩形框中：
        </p>
        <div id="div01" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
        <br/>
        <img id="drag01" src="../res/img/p001.png" draggable="true" ondragstart="drag(event)" width="336" height="200">
    </body>
</html>
```

> 设置元素为可拖放：
>
> ```html
> <img draggable="ture">
> ```
>
> ondragstart属性调用一个当对象被开始拖动时会触发的函数。
>
> ```hml
> ondragstart="drag(event)"
> ```
>
> drag(event)规定被拖动的数据。
>
> dataTransfer.setData()方法设置被拖动数据的数据类型和值。
>
> ```html
> function drag(ev) {
> ev.dataTransfer.setData("Text", ev.target.id);
> }
> ```
>
> ondragover属性调用一个当对象被**准备**放置拖动物时会触发的函数。
>
> ```html
> ondragover="allowDrop(event)"
> ```
>
> 默认地，无法将数据/元素放置到其他元素中。故我们必须阻止对元素的默认处理方式，这时要调用`event.preventDefault()`方法。
>
> ondrop属性调用一个当对象被放置拖动物时会触发的函数。
>
> ```html
> ondrop="drop(event)"
> ```
>
> 



# HTML5博客

```html
<!DOCTYPE html>
<html>
    <head>
        <title>星痕墨迹</title>
    </head>
    <body>
        <h2>
            <span>about me</span>
        </h2>
        <p>
            hi!I am a <b>W3Cschool</b> student.Code changes my world!
        </p>
        <p class="quote">
            "I love coding,I love w3cschool!"
        </p>
        <div class="section">
            <h1>
                <span>my media</span>
            </h1>
            <iframe height="150" width="300" src="https://www.w3cschool.cn/statics/demosource/movie.mp4" allowfullscreen frameborder="0">
</iframe>
        </div>
        <h1>
            <span>my skills</span>
        </h1>
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
        <h1>
            <span>my time table</span>
        </h1>
        <table>
            <tr>
            	<th>Day</th>
                <th>Mon</th>
                <th>Tue</th>
                <th>Wed</th>
                <th>Thu</th>
                <th>Fri</th>
            </tr>
            <tr>
            	<td>8:00-8:30</td>
                <td class="selected">Learn</td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
            	<td>9:00-10:00</td>
                <td></td>
                <td class="selected">Practice</td>
                <td></td>
                <td></td>
                <td></td>
            </tr>
            <tr>
            	<td>13:00-13:30</td>
                <td></td>
                <td></td>
                <td class="selected">Play</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
            	<td>15:45-17:00</td>
                <td></td>
                <td></td>
                <td></td>
                <td class="selected">Code</td>
                <td></td>
            </tr>
            <tr>
            	<td>18:00-18:15</td>
                <td></td>
                <td></td>
                <td></td>
                <td></td>
                <td class="selected">Discuss</td>
            </tr>
        </table>
        <h1>
            <span>contact me</span>
        </h1>
        <form>
            <input name="name" type="text" /><br/>
            <input name="email" type="email" /><br/>
            <textarea name="message"></textarea><br/>
            <input type="submit" value="send" class="submit" />
        </form>
    </body>
</html>
```



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




# CSS选择器

> note: 
>
> - 据点“.”表示class（可理解为后缀）
> - 井号“#”表示id
> - 空格“ ”表示后代
> - 大于号“>”表示子代

## 元素选择器

> **元素选择器**是指用**HTML标签名**作为选择器，按**标签名称**分类，为页面中某一类标签制定统一的CSS样式。

```html
<style type="text/css">
    div {
        color:red;
    }
</style>
```

## class选择器

> **class选择器（类型选择器）**通过绑定HTML元素上已设置的class标签进行设置对应的CSS样式。
>
> class前加.号

```html
<html>
    <head>
        <style type="text/css">
            .green {
                color:green;
            }
        </style>
    </head>
    <body>
        <div class="green">
            I am green,right?
        </div>
    </body>
</html>
```

## id选择器

> **id选择器**通过绑定HTML元素上已设置的唯一id标签进行设置对应的CSS样式。
>
> id前加#号。

```html
<html>
    <head>
        <style type="text/css">
            #blue {
                color:blue;
            }
        </style>
    </head>
    <body>
        <div id="blue">
            I am blue.Yes,I am so sad that I cann't be myself.
        </div>
    </body>
</html>
```

> id属性在文档内必须是唯一的。
>
> 不能使用数字开头的id属性！

## 后代选择器

> **后代选择器**选择某个父级下的所有子级，并针对该子级设置CSS样式。
>
> 父元素与子元素间加空格。

```html
<html>
    <head>
        <style type="text/css">
			.baby {
                color:black;
            }
            .father .baby {
                color:red;
            }
            .mother .baby {
                color:blue;
            }
            .grandpa .father .baby {
                color:green;
            }
			.grandpa .baby {
				color:#808000;
			}
        </style>
    </head>
    <body>
        <!-- 后代选择器 -->
        <p class="baby">
            .baby is black.
        </p>
        <div class="father">
            <p class="baby">
                .father .baby is red.
            </p>
        </div>
        <div class="mother">
            <p class="baby">
                .mother .baby is blue.
            </p>
        </div>
        <div class="grandpa">
            <div class="father">
                <p class="baby">
                    .grandpa .father .baby is green.
                </p>
            </div>
        </div>
        <div class="grandpa">
            <div class="mother">
                <p class="baby">
                    .grandpa .mother .baby is brown, because .grandpa .baby's definition is behind .mother .baby's!<br/>If you put .grandpa .baby's definition before .mother .baby's, then I will turn blue.
                </p>
            </div>
        </div>
    </body>
</html>
```

> 后代标签允许跨代影响。如：`.grandpa .baby {color:#808000;}`会对`<div class="grandpa"><div class="anyone"><p class="baby">I am brown.</p></div></div>`有作用。
>
> 不同的后代的标签可能会对同一处地方产生作用，此时谁的定义在后面便由谁！

## 子元素选择器

> **子元素选择器**与后代选择器类似，但不允许跨代影响。
>
> 父元素与子元素间加 > 号。

```html
<html>
    <head>
        <style type="text.css">
        	div > p {
        		color:red;
        	}
        	.mother > .baby {
        		color:blue;
        	}
        </style>
    </head>
    <body>
        <div>
            <p>
                p of div is red.
            </p>
        </div>
        <div class="mother">
            <p class="baby">
                baby of mother is blue.
            </p>
        </div>
        <div>
            <a href="C:\windows\system32\cmd.exe">
            	<p>
                    p, the grandson of div, is undefined.
                </p>
            </a>
        </div>
    </body>
</html>
```

## 相邻选择器

> **相邻选择器**选中对应元素的下一个兄弟元素。

```html
<html>
    <head>
        <style type="text/css">
            #w3cschool+p {
                color:red;
            }
            #error+p {
                color:blue;
            }
        </style>
    </head>
    <body>
        <div id="w3cschool">
            coding...
        </div>
        <p>
            coding after id w3cschool...
        </p>
        <p>
            coding after a long time since learning w3cschool...
        </p>
        <!-- coming is a intentional error -->
        <div id="error">
            coding when there is a bug...
        </div>
        <div>
            <!-- this p is not next to id error -->
            <p>
                coding when i found the bug...
            </p>
        </div>
    </body>
</html>
```

## 属性选择器

> **属性选择器**检索HTML页面中符合所设置的属性条件的元素。
>
> 属性选择器通过[]设置被选元素的属性条件。其中包含**属性名称**，后跟**可选条件**以匹配属性的值。如`img[alt] {width:80px; height:90px; }`将选择HTML页面中所有包含了alt属性的img元素并为其设置CSS样式。
>
> 属性选择器分两类：
>
> - 存在和值属性选择器（匹配精确的属性值）
>
>   - [attr]：包含attr属性的所有元素
>
>     `div[id] {color:red; }`
>
>   - [attr=val]：选择属性attr被赋值为val的所有元素
>
>     `a[href="http://testftp002.tech:404"] {color:red; }`
>
>   - [attr~=val]：仅选择属性attr中，属性值包含val的所有元素
>
>     `div[class~="w3cschool"] {color:red; }`
>
> - 子串值属性选择器（伪正则选择器）
>
>   - [attr|=val]：选择attr属性的值是val或值以val-开头的元素
>   - [attr^=val]：选择attr属性的值以val开头（包括val）的元素
>   - [attr$=val]：选择attr属性的值以val结尾（包括val）元素
>   - [attr*=val]：选择attr属性的值中包含字符串val的元素

```html
<html>
    <head>
        <style type="text/css">
            *[class] {
                color:red;
            }
            /* class中以w3cschool-开头或等于w3cschool的所有元素 */
            *[class|="w3cschool"] {
                color:green;
            }
            /* class中以w3cschool开头（包括w3cschool）的所有p元素 */
            p[class$="w3cschool"] {
                color:blue;
            }
        </style>
    </head>
    <body>
        <div class="w3cschool-programmer">
            程序猿
        </div>
        <div class="w3cschool_product">
            产品鲸鲤
        </div>
        <p class="designer-w3cschool">
            设计狮
        </p>
        <p>
            单身狗
        </p>
    </body>
</html>
```

## 选择器分组

> **选择器分组**通过逗号“,”将需要复用同一套样式的多个元素进行分隔。

```html
<html>
    <head>
        <style type="text/css">
            a, p, div {
                color:red;
            }
        </style>
    </head>
    <body>
        <div id="w3cschool">
            i am a div.
        </div><br/>
        <p>
            i am a p.
        </p><br/>
        <a>i am a a.</a><br/>
        <span>i am a span.</span>
    </body>
</html>
```



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



# CSS属性

## CSS列表样式

### list-style-type属性

> list-style-type属性允许我们设置不同的列表项标记。
>
> - none：无标记。在使用ul/ol进行一些网页布局（如菜单）时候较常使用。
> - disc：【默认】实心圆。
> - circle：空心圆。
> - square：实心方块。
> - decimal：数字。
> - decimal-leading-zero：0开头的数字（01， 02， 03等）。
> - lower-roman：小写罗马数字。
> - upper-roman：大写罗马数字。
> - lower-alpha：小写英文字母。
> - upper-alpha：大写英文字母。

### list-style-image属性

> list-style-image属性设置图像为列表中的项目标记。

### list-style-position属性

> list-style-position属性指定标记框的位置。
>
> `list-style-position: inside | outside; `

```html
<html>
    <head>
        <style type="text/css">
            ul {
                list-style-image: url("img/0005.ico"); 
                list-style-position: inside; 
            }
        </style>
    </head>
    <body>
        <p>
            以下列使用list-style-position: <b>inside</b> 属性。
        </p>
        <ul>
            <li>w3cschool01</li>
            <li>w3cschool02</li>
            <li>w3cschool03</li>
        </ul>
    </body>
</html>
```

### list-style属性

> `list-style: list-style-type list-style-position list-style-image; `

## CSS表格样式

### table属性

> `border-collapse: collapse | separete | inherit; `
>
> - collapse：如果可能，边框会合并为单一的边框。忽略border-spacing和empty-cells属性。
> - separate：【默认】边框会被分开。
> - inherit：从父元素继承。

```html
<html>
    <head>
        <style type="text/css">
            table {
                border-collapse: separate;
                border-spacing: 20px 40px; 
            }
        </style>
    </head>
    <body>
        <table border="5">
            <tr>
            	<td>a_11</td>
                <td>a_12</td>
                <td>a_13</td>
            </tr>
            <tr>
            	<td>a_21</td>
                <td>a_22</td>
                <td>a_23</td>
            </tr>
            <tr>
            	<td>a_31</td>
                <td>a_32</td>
                <td>a_33</td>
            </tr>
        </table>
    </body>
</html>
```

### caption-side属性

> caption-side属性指定表标题的位置。
>
> `caption-side: top | bottom;`

### empty-cells属性

> empty-cells属性设置是否显示表格中的空单元格（仅用于“分离边框”模式）。
>
> `empty-cells: show | hide | inherit; `

```html
<html>
    <head>
        <style type="text/css">
            table {
                border-collapse: separate;
                empty-cells: hide; 
            }
        </style>
    </head>
    <body>
        <table border="5">
            <tr>
                <td>HTML</td>
                <td>CSS</td>
            </tr>
            <tr>
                <td>JavaScript</td>
                <td></td>
            </tr>
        </table>
    </body>
</html>
```

<table border="5"  border-collapse="separate" empty-cells="hide">
    <tr>
    	<td>HTML</td>
        <td>CSS</td>
    </tr>
    <tr>
    	<td>JavaScript</td>
        <td></td>
    </tr>
</table>

### table-layout属性

> table-layout属性指定如何计算表格列的宽度。
>
> `table-layout: auto | fixed; `
>
> - auto：【默认】列宽度由单元格内容设定。
> - fixed：列宽由表格宽度和列宽度设定。

```html
<html>
    <head>
        <style type="text/css">
            table {
                border-collapse: separate; 
                width: 100%; 
                border: 1px solid green; 
            }
            td {
                border: 1px solid green; 
            }
            table.auto {
                table-layout: auto; 
            }
            table.fixed {
                table-layout: fixed; 
            }
        </style>
    </head>
    <body>
        <p>
            Table-layout is set to <b>auto</b>.
        </p>
        <table class="auto">
            <tr>
            	<td width="10%">500.000.000.000.000</td>
                <td width="90%">20.000</td>
            </tr>
        </table>
        <p>
            Table-layout is set to <b>fixed</b>.
        </p>
        <table class="fixed">
            <tr>
            	<td width="10%">500.000.000.000.000</td>
                <td width="90%">20.000</td>
            </tr>
        </table>
    </body>
</html>
```

## CSS链接样式

> 链接可以使用任何CSS属性（如color，font-family，background等）来设置样式。
>
> 依以下顺序依次设置：
>
> - a: link 定义普通的、未被访问的链接。
> - a: visited 定义访问后的链接。
> - a: hover 定义鼠标指针位于连接上方时刻。
> - a: active 定义链接被点击的时刻。

```html
<html>
    <head>
        <style type="text/css">
            a: hover {
                color: red; 
            }
        </style>
    </head>
    <body>
        <p>
            <a href="http://127.0.0.1" target="_blank">here is 80 port in your computer</a>
        </p>
    </body>
</html>
```

<p><a a:hover="red" href="http://127.0.0.1" target="_blank">here is 80 port in your computer</a></p>

### 文本链接的样式

> `text-decoration: none; `可以删除下划线。
>
> `border: none; `从包含连接的图像中删除边框。
>
> `outline: none; `删除IE中点击链接行上的虚线边框。

## CSS自定义鼠标光标样式

### cursor参数值

> cursor属性规定要显示的光标的类型（形状）。该属性定义了鼠标指针放在一个元素边界范围内时所用的光标形状。

\![0006]\(img/0006.jpg)

![0006](https://i.loli.net/2021/01/29/ybWl2Pa9GdMpgJL.jpg)

```html
<span style="cursor: help; ">need help?</span>
```

<span style="cursor: help; ">need help?</span>

```html
<html>
    <body>
        <p style="cursor: auto; ">
            The cursor of this paragraph has been set to auto.
        </p>
        <p style="cursor: move; ">
            The cursor of this paragraph has been set to move.
        </p>
        <p style="cursor: wait; ">
            The cursor of this paragraph has been set to wait.
        </p>
        <p style="cursor: pointer; ">
            The cursor of this paragraph has been set to pointer.
        </p>
        <p style="cursor: no-drop; ">
            The cursor of this paragraph has been set to no-drop.
        </p>
        <p style="cursor: s-resize; ">
            The cursor of this paragraph has been set to s-resize.
        </p>
        <p style="cursor: crosshair; ">
            The cursor of this paragraph has been set to crosshair.
        </p>
        <p style="cursor: text; ">
            The cursor of this paragraph has been set to text.
        </p>
        <p style="cursor: progress; ">
            The cursor of this paragraph has been set to progress.
        </p>
        <p style="cursor: not-allowed; ">
            The cursor of this paragraph has been set to not-allowed.
        </p>
    </body>
</html>
```



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











# CSS3基础

## CSS3简介

> 最重要的新功能：
>
> - **过渡**-允许设置效果曲线延迟时间等。
> - **形状转换**-允许元素2D或3D的切换。
> - **边界半径**-允许为元素创建圆角。
> - **边框图片**-允许我们指定一个图像作为元素周围的边框。
> - **多个背景**-将多个背景替换元素。
> - **动画**
> - **特效**

## CSS3前缀

> CSS3前缀用于去分别兼容各大主流浏览器对于CSS3新功能的支持。
>
> 各浏览器的**内核**：
>
> - IE——trident
> - Opera——Blink（presto已废弃）
> - Chrome——Blink（之前是webkit）
> - Firefox——Gecko
> - Safari——webkit
> - （Android手机使用频率最高的也是webkit内核）
>
> 每个内核的**前缀**：
>
> - Trident—— -ms-（代表IE私有属性）
> - Gecko—— -moz-（代表Firefox私有属性）
> - Presto—— -o-（代表Opera私有属性）
> - Webkit—— -webkit-（代表Chrome和Safari私有属性）

\![0001]\(img/0001.jpg "各浏览器的前缀列表")

![0001](https://i.loli.net/2021/01/29/nOMAtINszjBp8iW.jpg "各浏览器的前缀列表")

```html
<html>
    <head>
        <style type="text/css">
            div {
                border: 1px solid green; 
                -webkit-border-radius: 24px; 
            }
        </style>
    </head>
    <body>
        <div>
            W3Cschool
        </div>
    </body>
</html>
```

<div style="border: 1px solid green; -webkit-border-radius: 24px; ">
    W3Cschool
</div>

## CSS3圆角

### border-radius属性

> border-radius属性为任何元素设置**圆角**。
>
> - 四个值：左上    右上    右下    左下
> - 三个值：左上    右上与左下    右下
> - 两个值：左上与右下    右上与左下
> - 一个值：四个角

```html
<html>
    <head>
        <style type="text/css">
            div {
                width: 150px; 
                height: 50px; 
                margin: 5px; 
                background-color: green; 
                color: white; 
                text-align: center; 
                line-height: 50px; 
                display: inline-block; 
            }
            .div1 {
                border-radius: 20px; 
                background-color: blue; 
            }
            .div2 {
                /* border-radius的单位还可以是% */
                border-radius: 40%; 
                background-color: red; 
            }
        </style>
    </head>
    <body>
        <div class="div1">
            w3cschool
        </div>
        <div class="div2">
            w3cschool
        </div>
    </body>
</html>
```

<div style="width: 150px; height: 50px; margin: 5px; background-color: blue; color: white; text-align: center; line-height: 50px; display: inline-block; border-radius: 20px; ">
    w3cschool
</div>

<div style="width: 150px; height: 50px; margin: 5px; background-color: red; color: white; text-align: center; line-height: 50px; display: inline-block; border-radius: 20px; ">
    w3cschool
</div>

## CSS3阴影

### box-shadow属性

> box-shadow属性把一个或多个下拉阴影添加到框上。
>
> `box-shadow: h-shadow v-shadow blur spread color inset; `
>
> - h-shadow：【必需】水平阴影的位置，允许负值。
> - v-shadow：【必需】垂直阴影的位置，允许负值。
> - blur（模糊）：【可选】模糊距离。
> - spread（扩散）：【可选】阴影的尺寸。
> - color：【可选】阴影的颜色。
> - inset：【可选】从外侧的阴影（开始时）改变阴影内侧阴影。

```html
<html>
    <head>
        <style type="text/css">
            div {
                width: 300px; 
                height: 100px; 
                background-color: #9acd32; 
                box-shadow: 10px 10px #888888; 
            }
        </style>
    </head>
    <body>
        <div>
            W3Cschool
        </div>
    </body>
</html>
```

<div style="width: 300px; height: 100px; background-color: #9acd32; box-shadow: 10px 10px #888888; ">
    W3Cschool
</div>

```html
<html>
    <head>
        <style type="text/css">
            div {
                width: 300px; 
                height: 100px; 
                background-color: #9acd32; 
                box-shadow: 10px 10px 5px 5px #888888; 
            }
        </style>
    </head>
    <body>
        <div>
            W3Cschool
        </div>
    </body>
</html>
```

<div style="width: 300px; height: 100px; background-color: #9acd32; box-shadow: 10px 10px 5px 5px #888888; ">
    W3Cschool
</div>

## CSS3内阴影

> 默认阴影在边框外，使用inset后，阴影在边框内（即使是透明边框），背景之上内容之下。

```html
<html>
    <head>
        <style type="text/css">
            div {
                width: 300px; 
                height: 100px; 
                background-color: #9acd32; 
                box-shadow: 10px 10px 5px 5px #888888 inset; 
            }
        </style>
    </head>
    <body>
        <div>
            W3Cschool
        </div>
    </body>
</html>
```

<div style="width: 300px; height: 100px; background-color: #9acd32; box-shadow: 10px 10px 5px 5px #888888 inset; ">
    W3Cschool
</div>

> 可以通过使用逗号“,”来定义多个阴影。

## CSS3透明

> RGBA(R, G, B, A)
>
> - R, G, B：红、绿、蓝值，可以是整数或百分数。
> - A：透明度，取值0~1之间。

\![0002]\(img/0002.jpg)

![0002](https://i.loli.net/2021/01/29/ohIslVUiOMNnWyv.jpg)

```html
<html>
    <head>
        <style type="text/css">
            body {
                background: url("https://www.w3cschool.cn/attachments/image/20180125/1516870677823170.jpg"); 
            }
            nav {
                padding: 50px 0; 
                min-width: 500px; 
            }
            nav ul {
                background: linear-gradient(90deg, 
                rgba(255, 255, 255, 0) 0%, 
                rgba(255, 255, 255, 0.2) 25%, 
                rgba(255, 255, 255, 0.2) 75%, 
                rgba(255, 255, 255, 0) 100%); 
                box-shadow: 0 0 25px rgba(0, 0, 0, 0.1), 
                    0 0 1px rgba(255, 255, 255, 0.6) inset; 
            }
            nav ul li {
                display: inline-block; 
            }
            nav ul li a {
                padding: 10px; 
                color: #ffffff; 
                font-size: 18px; 
                font-family: Arial; 
                text-decoration: none; 
                display: block; 
            }
        </style>
    </head>
    <body>
        <nav>
        	<ul>
                <li><a href="http://testftp002.tech">星痕墨迹</a></li>
                <li><a href="http://testftp002.tech:404">code代码仓库</a></li>
                <li><a href="http://testftp002.tech:6080">mail</a></li>
                <li><a href="http://127.0.0.1">your web</a></li>
            </ul>
        </nav>
    </body>
</html>
```

<div width="100%" height="300px" style="background: url('https://www.w3cschool.cn/attachments/image/20180125/1516870677823170.jpg');">
    <nav style="padding: 100px 0;  min-width: 500px; " >
<ul style="background: linear-gradient(90deg, rgba(255, 255, 255, 0) 0%, rgba(255, 255, 255, 0.2) 25%, rgba(255, 255, 255, 0.2) 75%, rgba(255, 255, 255, 0) 100%); box-shadow: 0 0 25px rgba(0, 0, 0, 0.1), 0 0 1px rgba(255, 255, 255, 0.6) inset; ">
<li style="display: inline-block; "><a href="http://testftp002.tech" style="padding: 10px; color: #ffffff; font-size: 18px; font-family: Arial; text-decoration: none; display: block; ">星痕墨迹</a></li>
<li style="display: inline-block; "><a href="http://testftp002.tech:404" style="padding: 10px; color: #ffffff; font-size: 18px; font-family: Arial; text-decoration: none; display: block; ">code代码仓库</a></li>
<li style="display: inline-block; "><a href="http://testftp002.tech:6080" style="padding: 10px; color: #ffffff; font-size: 18px; font-family: Arial; text-decoration: none; display: block; ">mail</a></li>
<li style="display: inline-block; "><a href="http://127.0.0.1" style="padding: 10px; color: #ffffff; font-size: 18px; font-family: Arial; text-decoration: none; display: block; ">your web</a></li>
</ul>
</nav>
</div>

## CSS3文本阴影

### text-shadow属性

> `text-shadow: h-shadow v-shadow blur color; `
>
> - h-shadow：【必需】水平阴影的位置，允许负值。
> - v-shadow：【必需】垂直阴影的位置，允许负值。
> - blur：【可选】模糊的距离。
> - color：【可选】阴影的颜色。        
>
> 可以通过使用逗号“,”来定义多个阴影。

```html
<html>
    <head>
        <style type="text/css">
            h1 {
                text-shadow: 5px 10px 2px #93968f, 
                    -3px 6px 5px #58d1e3; 
            }
        </style>
    </head>
    <body>
        <h1>
            W3CSCHOOL
        </h1>
    </body>
</html>
```

<h1 style="text-shadow: 5px 10px 2px #93968f, -3px 6px 5px #58d1e3; ">
    W3CSCHOOL
</h1>

```html
<html>
    <head>
        <style type="text/css">
            body {
                background: #ccc; 
            }
            div {
                color: #ccc; 
                font: 500 80px "微软雅黑"; 
            }
            .div1 {
                text-shadow: 1px 1px 1px #000, 
                    -1px -1px -1px #fff; 
            }
            .div2 {
                text-shadow: -1px -1px -1px #000, 
                    1px 1px 1px #fff; 
            }
        </style>
    </head>
    <body>
        <div class="div1">
            凸起的文字
        </div>
        <div class="div2">
            凹下的文字
        </div>
    </body>
</html>
```

## CSS3伪类

> CSS3伪类用于向某些选择器添加特殊效果，它允许我们在不适用JavaScript等脚本的情况下去设置web页面中某些特定的元素的属性。
>
> 伪类通常以“:”（冒号）开头。
>
> - :first-child    将会匹配该元素中的第一个子元素。
> - :last-child    将会匹配该元素中的最后一个子元素。
> - :nth-child(n)    将会匹配该元素中的第n个子元素。
> - :nth-child(2n)    将会选择该元素中所有偶数子元素。
> - :nth-child(2n+1)    将会选择该元素中所有奇数子元素。

```html
<html>
    <head>
        <style type="text/css">
            #parent p:first-child {
                color: green; 
                text-decoration: underline;  
            }
            #parent p:last-child {
                color: pink; 
            }
            #parent p:nth-child(3) {
                color: blue; 
            }
            #parent p:nth-child(2n) {
                font-size: 14px; 
            }
            #parent p:nth-child(2n+1) {
                font-size: 22px; 
            }
        </style>
    </head>
    <body>
        <div id="parent">
            <p>
                First w3cschool
            </p>
            <p>
                Second w3cschool
            </p>
            <p>
                Third w3cschool
            </p>
            <p>
                Fourth w3cschool
            </p>
            <p>
                Fifth w3cschool
            </p>
        </div>
    </body>
</html>
```

## CSS3伪元素

> CSS伪元素是用来添加一些选择器的特殊效果。在CSS中有五个伪元素，都以双冒号“::”开头：
>
> - ::first-line    选择器中文本的第一行
> - ::first-letter    选择器中文本的第一个字母
> - ::selection    选择用户选择的元素部分
> - ::before    在元素之前插入一些内容
> - ::after    在元素之后插入一些内容

```html
<html>
    <head>
        <style type="text/css">
            p::first-line {
                color: #ae4141; 
            }
            p::selection {
                background: blue; 
                color: #808000; 
            }
            /* 使用-moz-前缀是因为Mozilla不支持::selection元素 */
            p::-moz-selection {
                background: blue; 
                color: #808000; 
            }
        </style>
    </head>
    <body>
        <p>
            First w3cschool<br/>
            Second w3cschool<br/>
            Third w3cschool<br/>
            Fourth w3cschool
        </p>
    </body>
</html>
```

```html
<html>
    <head>
        <style type="text/css">
            p::before {
                content: url('img/0003.ico'); 
            }
        </style>
    </head>
    <body>
        <p>
            Firth w3cschool
        </p>
        <p>
            Second w3cschool
        </p>
        <p>
            Third w3cschool
        </p>
        <p>
            Fourth w3cschool
        </p>
    </body>
</html>
```

## CSS3自动换行

### word-wrap属性

> `word-wrap: normal | break-word; `
>
> - normal：只在允许的断字点换行（浏览器默认处理）。
> - break-word：在长单词或URL地址内部进行换行。

```html
<html>
    <head>
        <style type="text/css">
            p {
                width: 100px; 
                height: 100px; 
                border: 1px solid #000000; 
                word-wrap: normal; 
            }
        </style>
    </head>
    <body>
        <p>
            wwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwwww
        </p>
    </body>
</html>
```

## CSS3@font-face

> @font-face规则允许将自定义字体加载到网页中。
>
> `@font-face {font-family: name_of_your_font; src: url("example.ttf")}`

\![0004]\(img/0004.jpg "各浏览器所支持的字体文件")

![0004](https://i.loli.net/2021/01/29/U2VwpbN85iD7msy.jpg "各浏览器所支持的字体文件")








# CSS3渐变与背景

> gradients使你能够现实两个或多个指定颜色之间的平滑过渡。
>
> - 线性渐变（Linear）向下、上、左、右、对角线方向。
> - 径向（Radial）由他们的中心定义。

## 线性渐变

> 可以使用**十六进制**、**RGB**或**HSL**等来进行渐变定义。

```CSS
div {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: linear-gradient(DeepSkyBlue, White); 
}
```

<div style="float: left; width: 300px; height: 100px; margin: 4px; color: #fff; background: linear-gradient(DeepSkyBlue, White); ">
    w3cschool
</div>





### 颜色停止

> 线性渐变可以通过“, ”逗号分隔添加多个颜色，浏览器将有上到下的在几种颜色中生成颜色区间并生成渐变效果。

```CSS
div {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: linear-gradient(
        rgb(255, 0, 0),
        rgb(127, 127, 0), 
        rgb(0, 255, 0),
        rgb(0, 127, 127), 
        rgb(0, 0, 255),
        rgb(127, 0, 127)); 
}
```

<div style="float: left; width: 300px; height: 100px; margin: 4px; color: #fff; background: -webkit-linear-gradient(rgb(255, 0, 0), rgb(127, 127, 0), rgb(0, 255, 0), rgb(0, 127, 127), rgb(0, 0, 255), rgb(127, 0, 127)); ">
    w3cschool
</div>





```CSS
div {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    /* 颜色停止 */
    background: linear-gradient(Blue 20%, yellow 30%, green 85%); 
}
```

<div style="float: left; width: 300px; height: 100px; margin: 4px; color: #fff; background: linear-gradient(Blue 20%, yellow 30%, green 85%); ">
    w3cschool
</div>





> 除百分比外，还可以使用px，em等来指定颜色停止。
>
> 如果你对两种颜色使用相同的颜色停止位置，则会在他们之间创建一条清晰的线条。

> 渐变的方向是可以被改变的。
>
> `linear-gradient(top | right | bottom | left | bottom right | deg, color_01, color_02, ....)`
>
> - bottom：从下到上。
> - bottom right：对角线。
> - deg：0deg从左到右，90deg从下到上。

```CSS
div:first-child {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: -webkit-linear-gradient(left, blue, green, white); 
}
div:nth-child(2) {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: -webkit-linear-gradient(100deg, blue, green, white);
}
div:last-child {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: -webkit-linear-gradient(bottom, blue, green, white); 
}
```

<div>
    <div style="float: left; 
                width: 300px; 
                height: 100px; 
                margin: 4px; 
                color: #fff; 
                background: -webkit-linear-gradient(left, blue, green, white); ">
        w3cschool
    </div>
    <div style="float: left; 
                width: 300px; 
                height: 100px; 
                margin: 4px; 
                color: #fff; 
                background: -webkit-linear-gradient(100deg, blue, green, white);">
        w3cschool
    </div>
    <div style="float: left; 
                width: 300px; 
                height: 100px; 
                margin: 4px; 
                color: #fff; 
                background: -webkit-linear-gradient(bottom, blue, green, white); ">
        w3cschool
    </div>
</div>

















### 重复线性渐变

> repeating-linear-gradient()函数用于重复线性渐变

```CSS
div {
    float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: -webkit-repeating-linear-gradient(blue, green 20px); 
}
```

<div style="float: left; 
    width: 300px; 
    height: 100px; 
    margin: 4px; 
    color: #fff; 
    background: -webkit-repeating-linear-gradient(blue, green 20px); ">
    w3cschool
</div>





## 径向渐变

> `radial-gradient(shape size position, color_01, color_02, ....)`
>
> - shape：确定圆的类型：
>   - ellipse：【默认】椭圆径向渐变。
>   - circle：圆形径向渐变。
> - size：定义渐变的大小：
>   - farthest-corner：【默认】圆心到最远的角。
>   - closest-side：圆心到最近的边。
>   - closest-corner：圆心到最近的角。
>   - farthest-side：圆心到最远的边。
> - position：定义渐变的位置：
>   - center：【默认】设置中间为径向渐变圆心的纵坐标值。
>   - top：设置顶部为径向渐变圆心的纵坐标值。
>   - bottom：设置底部为径向渐变圆心的纵坐标值。
>   - 还可以使用关键字top right等或**长度值**、**百分比值**、**像素**、**ems**或组合起来定位。

```CSS
div div {
    height: 150px; 
    width: 200px; 
    color: #fff; 
}
div:first-child {
    background: -webkit-radial-gradient(top left, green, yellow, blue); 
}
div:nth-child(2) {
    background: -webkit-radial-gradient(green 5%, yellow 15%, blue 60%); 
}
```

<div>
    <div style="height: 150px; width: 200px; color: #fff; background: -webkit-radial-gradient(top left, green, yellow, blue); ">
        w3cschool
    </div>
    <div style="height: 150px; width: 200px; color: #fff; background: -webkit-radial-gradient(green 5%, yellow 15%, blue 60%); ">
        w3cschool
    </div>
</div>

### 颜色停止

<div style="width: 200px; height: 100px; background: -webkit-radial-gradient(circle, green 40%, yellow 50%, blue 70%); ">w3cschool</div>

## background-size

> background-size属性让我们能够用长度或百分比来指定背景图像的大小。
>
> `background-size: length | percentage | cover | contain; `
>
> - length：设置背景图像的宽度和高度。第一个值是宽度，第二个值是高度。如果只设置第一个值，那么第二个值会自动转换为auto。
> - percentage：以父元素的百分比来设置图片的宽度和高度。第一个值是宽度，第二个值是高度。如果只设置第一个值，那么第二个值会自动转换为auto。
> - cover：把背景图像扩展至足够大，以使背景图像完全覆盖背景区域。
> - contain：把图像扩展至最大尺寸，以使宽度和高度完全适应内容区域。

## background-clip

> background-clip属性指定背景的绘画区域。
>
> `background-clip: border-box | padding | content-box; `
>
> - border-box：【默认】背景被绘制到边框的外边缘。
> - padding-box：背景被绘制到填充的外边缘。
> - content-box：背景被绘制在内容框中。

```CSS
div div {
    border: 10px dashed blue; 
    padding: 20px;
    margin: 10px; 
    display: inline-block; 
    background: red; 
    color: white; 
}
div:first-child {
    background-clip: border-box; 
}
div:nth-child(2) {
    background-clip: padding-box; 
}
div:last-child {
    background-clip: content-box; 
}
```

<div>
    <div style="border: 10px dashed blue; 
    padding: 20px;
    margin: 10px; 
    display: inline-block; 
    background: red; 
    color: white;
    background-clip: border-box; ">
        w3cschool
    </div>
    <div style="border: 10px dashed blue; 
    padding: 20px;
    margin: 10px; 
    display: inline-block; 
    background: red; 
    color: white;
    background-clip: padding-box; ">
        w3cschool
    </div>
    <div style="border: 10px dashed blue; 
    padding: 20px;
    margin: 10px; 
    display: inline-block; 
    background: red; 
    color: white;
    background-clip: content-box; ">
        w3cschool
    </div>
</div>

> background-clip也适用于背景图片。

## 透明的边框

```html
<html>
    <head>
        <style type="text/css">
            body {
                background: url("https://www.w3cschool.cn/attachments/image/20180125/1516870677823170.jpg"); 
            }
            #first {
                border: 20px solid rgba(0, 0, 0, 0.2); 
                -moz-background-clip: padding-box; 
                background-clip: padding-box; 
                background-color: white; 
                display: inline-block; 
                width: 20%; 
            }
            #second {
				border: 20px solid rgba(0, 0, 0, 0.2); 
                background-color: white; 
                display: inline-block; 
                width: 20%; 
            }
            div a {
                text-decoration: none; 
                color: green; 
            }
        </style>
    </head>
    <body>
        <div id="first">
            <a href="http://testftp002.tech">星痕墨迹</a>
        </div>
        <div id="second">
            <a href="http://127.0.0.1">your web</a>
        </div>
    </body>
</html>
```

<div style="width: 100%; height: 300px; background: url('https://www.w3cschool.cn/attachments/image/20180125/1516870677823170.jpg'); ">
    <div style="border: 20px solid rgba(0, 0, 0, 0.2); 
                -moz-background-clip: padding-box; 
                background-clip: padding-box; 
                background-color: white; 
                display: inline-block; 
                width: 20%; ">
        <a href="http://testftp002.tech">星痕墨迹</a>
    </div>
    <div style="border: 20px solid rgba(0, 0, 0, 0.2); 
                background-color: white; 
                display: inline-block; 
                width: 20%; ">
        <a href="http://127.0.0.1">your web</a>
    </div>
</div>

## 层叠的背景图

> `background: url("example_01.png") position_01 repeat_01,  url("example_02.png") position_02 repeat_02, ....; `  
>
> 背景图中越前面的优先级越高。
>
> background-position属性值：
>
> \![0005]\(img/0005.jpg)
>
> ![0005](https://i.loli.net/2021/01/30/1tSLFfsQ7Ez8i3n.jpg)

```CSS
div {
    width: 400px; 
    height: 300px; 
    background-image: url("https://7nsts.w3cschool.cn/images/w3c/header-logo.png"), url("https://7n.w3cschool.cn/attachments/image/20180125/1516870677823170.jpg"); 
    background-position: right top, left top; 
    background-repeat: no-repeat; 
}
```

<div style="width: 400px; 
    height: 300px; 
    background-image: url('https://7nsts.w3cschool.cn/images/w3c/header-logo.png'), url('https://7n.w3cschool.cn/attachments/image/20180125/1516870677823170.jpg'); 
    background-position: right top, left top; 
    background-repeat: no-repeat; ">
    w3cschool
</div>

## opacity属性

> opacity属性可以设置不透明度。取值为0.0~1.0。
>
> 要让opacity属性兼容所有的IE版本，要同时使用`filter: alpha(opacity=100x); `和`opacity: x; `





# CSS3过渡与转换

## 转换

> CSS3转换（transition）允许我们在限定的时间内从一个属性值**转换**到另一个属性值。
>
> - transition-property：指定要转换的属性。
> - transition-duration：指定转换发生的持续时间。（为0时无过渡效果）
> - transition-timing-function：指定转换的速度在其持续时间内如何变化。
> - transition-delay：制定过渡效果的延迟（以秒为单位）。
>
> 默认值为`transition: all 0 ease 0; `

### transition-property

```CSS
div {
    width: 100px; 
    height: 100px; 
    background: red; 
    color: #fff; 
    transition: width 3s; 
}
div:hover {
    width: 250px; 
}
```

### transition-timing-function

> - ease：【默认】先缓慢后加速
>
> - ease-in：缓步开始，然后加速，再突然停止
>
> - ease-out：快速启动，减速停止
>
> - ease-in-out：类似于ease，但加减速稍微不同
>
> - linear：匀速变换
>
> - \<img src="img/0006.png" style="float: right; " />
>
>   <img src="https://i.loli.net/2021/01/30/kwg4VlFnpCSvMA5.png" style="float: right">cubic-bezier()函数：定义一个贝赛尔曲线（Cubic Bezier）。
>
>   贝塞尔曲线由四个点P0，P1，P2，P3定义。
>
>   取值范围0~1之间。
>
>   `transition-timing-function: cubic-bezier(0, 0, 1, 1); `

## transform

> CSS3中transform允许我们**翻转**，**旋转**，**缩放**和**倾斜**元素。

### transform-origin

> transform-origin属性允许我们更改**已转换元素**的位置。该属性的默认值是50% 50%，对应于元素的中间。

```CSS
div:first-child {
    position: relative; 
    height: 100px; 
    width: 100px; 
    margin: 30px; 
    padding: 10px; 
    border: 1px solid black; 
}
div:nth-child(2) {
    position: absolute; 
    padding: 50px; 
    border: 1px solid white; 
    background-color: #8bc34a; 
    transform: rotate(15deg); 
    transform-origin: 30% 80%; 
}
```

<div>
    <div style="position: relative; height: 100px; width: 100px; padding: 10px; border: 1px solid black; display: inline-block; ">
	</div>
	<div style="position: relative; padding: 50px; margin: -100px; border: 1px solid white; background-color: #8bc34a; transform: rotate(15deg); transform-origin: 30% 80%; display: inline-block; ">
w3cschool
    </div>
</div>



### rotate

> rotate()方法旋转当前的绘图。
>
> 旋转只会影响到旋转完成后的绘图。

```CSS
div {
    width: 200px; 
    height: 100px; 
    margin-top: 30px; 
    background-color: #32cd32; 
    transform: rotate(15deg); 
}
```

<div style="width: 200px; 
    height: 100px; 
    margin-top: 30px; 
    background-color: #32cd32; 
    transform: rotate(15deg); ">
    w3cschool
</div>

### translate

> translate()方法平移当前的绘图。

```CSS
div {
    padding: 50px; 
    position: absolute; 
    background-color: red; 
    transform: translate(120px, 60px); 
}
```

<div style="padding: 50px; 
    position: absolute; 
    background-color: red; 
    transform: translate(120px, 60px); ">
    w3cschool
</div>







### skew

> skew()方法通过给元素设置X轴和Y轴的倾斜角度值来实现倾斜。

```CSS
div {
    padding: 50px; 
    position: absolute; 
    background-color: blue; 
    transform: skew(45deg); 
    -webkit-transform: skew(45deg); 
}
```

<div style="padding: 50px; 
    position: absolute; 
    background-color: blue; 
    transform: skew(45deg); 
    -webkit-transform: skew(45deg); ">
    w3cschool
</div>







### scale

> scale()方法用于缩放

> 多重transform间用空格隔开。

## 动画

### @keyframes规则

```CSS
div {
    width: 100px; 
    height: 100px; 
    background-color: red; 
    animation-name: example; 
    animation-duration: 1s; 
}
@keyframes example {
    /* 也可以使用from（0%）和to（100%）关键字 */
    0% {background-color: red; }
    50% {background-color: yellow; }
    70% {background-color: blue; }
    100% {background-color: green; }
}
```

### 动画属性

> animation-timing-function指定动画的速度曲线：
>
> - ease：【默认】慢启动，然后快速，再慢慢结束。
> - linear：匀速。
> - ease-in：慢启动。
> - ease-out：慢结束。
> - ease-in-out：慢启动、慢结束。
> - cubic-bezier(n, n, n, n)：n取值为0~1。
>
> animation-delay属性定义动画何时开始。
>
> animation-iteration-count属性指定动画重复次数。（无限次为infinite）
>
> animation-direction属性指定如何应用关键帧：
>
> - normal：【默认】从0%到100%前进。
> - reverse：从100%到0%。
> - alternate：先向前，后向后，再向前。
> - alternate reverse：先向后，后向前，再向后。

> `animation: animation-name animation-duration animation-timing-function animation-dalay animation-iteration-count animation-direction; `

## 3D转换

> `transform: translate3d(x, y, z) rotate3d(x_deg, y_deg, z_deg) `
>
> - `translate3d(x, y, z)`等价于`translateX(x) translateY(y) translateZ(z)`
> - `rotate3d(x, y, z)`等价于`rotateX(x) rotateY(y) rotateZ(z)`
>
> prespective定义如何渲染3D场景的深度。

```CSS
div.empty-div {
    position: relative; 
    height: 200px; 
    width: 200px; 
    margin: 30px; 
    padding: 10px; 
    border: 1px solid black; 
    perspective: 100px; 
    -webkit-perspective: 100px; 
}
div.red-div {
    padding: 60px; 
    position: absolute; 
    background-color: red; 
    border: 1px solid white; 
    transform: rotateX(45deg); 
    -webkit-transform: rotateX(45deg); 
}
```

<div style="position: relative; height: 200px; width: 200px; margin: 30px; padding: 10px; border: 1px solid black; perspective: 100px; -webkit-perspective: 100px; ">
    <div style="padding: 60px; position: absolute; background-color: red; border: 1px solid white; transform: rotateX(45deg); -webkit-transform: rotateX(45deg); "></div></div>





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


# JavaScript基本概念

### 语句

> 语句（statement）是为了完成某种任务而进行的操作。
>
> 语句以分号结尾。

### 变量

> 变量是用于存储信息的容器，变量的值可以在整个程序中被修改。
>
> 变量使用关键字var来声明， 初始值为undefined。
>
> JavaScript区分大小写。 

> typeof运算符用来监测一个变量的类型，返回一个字符串。

#### 变量提升

> JavaScript引擎先解析代码，获取所有被声明的变量，然后再一行行地运行。也就是说，所有变量的声明语句都会被提升到代码的头部， 这就叫做**变量提升（hoisting）**。

> `console.log(a); var a = 1; `不会报错， 但真正运行的是`var a; console.log(a); a = 1; `，最后的结果是显示undefined！

### 区块

> JavaScript使用大括号将多个相关语句组合在一起，称为区块（block）。
>
> 对于var命令来说，JavaScript的区块不构成单独的作用域（scope）。如`{var a = 1; } document.write(a); // 1`中var在区块内，但在区块外依然有效。

### 数据类型

> JavaScript有五种数据类型：
>
> - 字符串（string）
> - 数字（number）
> - 布尔（boolean）
> - 空（null）
> - 未定义（undefined）
> - 对象（object）
> - symbol【新增】

#### null与undefined

> null是一个表示“空”的对象（typeof null == object），转为数值时为0； 
>
> undefined是一个表示“此处无定义”的原始值（typeof undefined == undefined），转为数值时为NaN。

#### boolean

> 下列运算符会返回布尔值：
>
> - 两元逻辑运算符：&&(And), ||(Or)
> - 前置逻辑运算符：!(Not)
> - 相等运算符：===, !==, ==, !=
> - 比较运算符：>, >=, <, <=
>
> 若JavaScript预期某个位置应该是布尔值，则会自动将值转为布尔值。转换规则是除下列六个值被转为false外，其他值都视为true【特别注意空数组（[]）和空对象（{}）对应布尔值为true】：
>
> - undefined
> - null
> - false
> - 0
> - NaN
> - ""或''（空字符串）

#### number

> JavaScript只有一种数值类型，数值可以带小数点也可不带。

#### string

> 字符串用双引号""或单引号''包裹。
>
> 用反斜杠\转义。

### 三元运算符

> `(条件) ? 表达式1 : 表达式2`如果“条件”为true则返回“表达式1”的值， 否则返回“表达式2”的值。

### 比较运算符

给定x=5，有如下结果：

\![0001]\(img/0001.jpg)

![0001](https://i.loli.net/2021/01/30/FSOvQ7KVI2oyXY8.jpg)

### 赋值运算符

\![0002]]\(img/0002.jpg)

![0002](https://i.loli.net/2021/01/30/6h3al5tsgWmOSRL.jpg)

### 字符串

> 字符串是可检索的。

>  特殊字符
>
> - \n：换行
> - \r：回车
> - \t：tab（制表符）
> - \b：退格符
> - \f：换页符

> 使用length来计算字符串长度。

> 字符串运算符：
>
> +符号连接字符串

> 字符串的不变性：
>
> JavaScript中字符串一旦被创建就不能被修改。






# JavaScript条件和循环

### if-else if-else语句

```javascript
if (条件01) {
    // 条件01为true时会执行的代码 
}
else if (条件02) {
    // 条件01位false且条件02位true时会执行的代码
}
else {
    // 条件01和条件02都为flase时会执行的代码
}
```

### switch语句

```JavaScript
switch(表达式) {
    case 结果1:
        // 表达式==结果1时会执行的代码
        break; 
    case 结果2:
        // 表达式==结果2时会执行的代码
        break; 
    ...
    case 结果n:
        // 表达式==结果n时会执行的代码
        break; 
    default:
        // 表达式与上述所有结果不等时会执行的代码
}
```

### for循环

```JavaScript
/*
Statement01：在循环开始前执行； 
Statement02：定义运行循环的条件； 
Statement03：在执行循环后都会执行； 
*/
for (Statement01; Statement02; Statement03) {
    // 循环执行的代码
}
```

### while循环

```JavaScript
while (条件) {
    // 只要“条件”为true就会执行的代码
}
```

### do while循环

```JavaScript
do {
    // 有可能被循环执行的代码（当“条件”为true时）
}
while (条件); 
```

### break与continue语句

> break语句用于跳出当前循环； 
>
> continue语句跳出循环后会继续执行循环之后的代码； 

### JS标签

> JavaScript允许语句前面设置标签（label）相当于定位符，用于跳转到程序的任意位置。
>
> `label: 语句`标签可以是任意非保留字的标识符，语句部分可以是任意语句。

> 标签通常与break语句和continue语句配合使用，跳出特定的循环。

```JavaScript
// 跳出双层循环
label01: for (var i = 0; i < 3; i++) {
    for (var j = 0; j < 3; j++) {
        if (i === 1 && j === 1) break label01; 
        console.log("i=" + i + ", j=" + j + "; "); 
    }
}// i=0, j=0; i=0, j=1; i=0, j=2; i=1, j=0; 
```

```JavaScript
// 跳出区块
label02: {
    console.log("本行正常输出"); 
    break label02; 
    console.log("本行不会输出"); 
}
console.log("本行也正常输出"); 
```





# JavaScript函数

### 函数定义

```JavaScript
function functionName(parameters) {
    // 函数中的代码
}
```

### 函数参数

> 函数显式参数在函数定义时列出，函数隐式参数arguments是函数调用时传递给函数真正的值。如
>
> ```JavaScript
> function sum() {
>  return arguments[0] + arguments[1]; 
> }
> sum(1, 2); //3
> ```
>
> 参数规则：
>
> - JavaScript函数定义时参数没有指定数据类型；
> - JavaScript函数对隐藏参数（arguments）没有进行检测；
> - JavaScript函数对隐藏参数（arguments）的个数没有进行检测。
>
> 多参数用逗号“, ”分隔，调用函数时如果缺少参数，则缺少值为undefined。

### 变量作用域

> **作用域**是可访问变量的集合。【在JavaScript中，**对象**和**函数**同样是变量】
>
> JavaScript局部作用域：
>
> - 变量在函数内声明，变量为局部作用域，局部变量只能在函数内部访问。
> - 局部变量在函数开始执行时创建，函数执行完后局部变量会自动销毁。
> - 局部变量的优先级高于同名的全局变量。
>
> JavaScript全局变量：
>
> - 变量在函数外定义即全局变量，全局变量网页中所有脚本和函数均可使用。
>
> - <span style="color: #800000">如果变量在函数内没有声明（没有使用var关键字），则该变量为全局变量。</span>如：
>
>   ```JavaScript
>   // 此处可调用carName变量
>   
>   function myFunction() {
>       carName = "大众"; 
>       // 此处carName为全局变量！
>   }
>   ```
>
> - 全局变量在页面关闭后销毁。
>
> HTML中的全局变量：
>
> - 在HTML中，全局变量是**window**对象：**所有数据变量都属于window对象**。
>
>   ```JavaScript
>   // 此处可用window.carName
>   
>   function myFunction() {
>       carName = "大众"; 
>   }
>   ```

### 弹出框

> JavaScript提供三种类型的弹出框：
>
> - Alert
> - Prompt
> - Confirm

#### Alert警告框

> 当弹出警告框时，用户必须单击“确定”以继续。
>
> 警报功能采用单个参数，即弹出框中显示的文本。
>
> 使用alert弹出框，将阻塞整个页面的运行，点击确定后才继续运行。

```JavaScript
alert("Hello World!"); 
```

\![0003]\(img/0003.png)

![0003](https://i.loli.net/2021/01/31/LpGtYjkcKOSdNr9.png)

#### Prompt框

> 通常使用Prompt框来让用户输入一个值。
>
> 当弹出提示框（Prompt框）时，输入输入值后，用户将不得不单击“确定”或“取消”以继续。
>
> 如果用户单击确定，该框将返回输入值；如果用户单击取消，该框将返回null。
>
> Prompt()方法有两个参数：
>
> - 第一个是要在文本框中显示的标签
> - 第二个是在文本框中显示的默认字符串【可选】

```JavaScript
var input = prompt("so embarrassed, em...ok, input something: ", "Hurry up!"); 
alert(input); 
```

\![0004]\(img/0004.png)

![0004](https://i.loli.net/2021/01/31/5sUpaViSQnywY6q.png)

#### Confirm框

> 通常使用Confirm框让用户验证或接受某些内容。
>
> 当弹出确认框（Confirm框）时，用户必须单击“确定”或“取消”以继续。
>
> 如果用户单击确定，该框将返回true；如果用户单击取消，该框将返回false。

```JavaScript
var result = confirm("Are you sure to leave?"); 
if (result === true) {
    alert("get away!"); 
}
else {
    alert("I have bet it!"); 
}
```

\![0005]\(img/0005.png)

![0005](https://i.loli.net/2021/01/31/gitsyVXBTJWUnlI.png)




# JavaScript对象

> JavaScript对象是拥有属性和方法的数据。
>
> JavaScript中的一切皆对象：字符串、数值、数组、函数....此外，JavaScript也允许自定义对象。

### 对象定义

```JavaScript
var myObject = {
    name01: value01, name02: value02, ...
}
```

> 其中，myObject即对象，name为对象的属性，value为对象属性对应的值。如：

```JavaScript
var person = {
    name: "John", age: 31, favColor: "green", height: 183, 
}; 
```

### 对象属性

> 可以通过`objectName.propertyName`或`objectName["propertyName"]`访问对象属性。

### 对象构造器

```JavaScript
function person(firstname, lastname, age, eyecolor) {
    this.firstname = firstname; 
    this.lastname = lastname; 
    this.age = age; 
    this.eyecolor = eyecolor; 
}
```

> this通常指向我们正在执行的函数本身，或该函数所属的对象。

#### 创建JavaScript对象实例

```JavaScript
var myFather = new person("John", "Doe", 50, "blue"); 
var myMother = new person("Sally", "Rally", 48, "green"); 
```

### 对象初始化

> 使用英文大括号{}创建**单个**对象：
>
> ```JavaScript
> var John = {name: "John", age: 25}; 
> var Loen = {name: "Loen", age: 28};  
> ```

### 添加方法

> 方法是存储在对象属性中的函数。
>
> 创建对象函数：`methodName: function(paraments) { code lines }`; 
>
> 使用`objectName.methodName()`访问对象函数。

```JavaScript
function person(name, age) {
    this.name = name; 
    this.age = age; 
    this.changeName = function (name) {
        this.name = name; 
    }
}

var p = new person("Loen", 28); 
p.changeName("John"); 
```

> 我们也可以在构造函数外定义一个函数，通过函数名关联到对象的属性上：【注意将函数关联到对象属性时不需要写括号】

```JavaScript
function person(name, age) {
    this.name = name; 
    this.age = age; 
    this.yearOfBirth = bornYear; // 关联到bornYear函数
}
function bornYear() {
    return new Date().getFullYear() - this.age; 
}
```





# JavaScript数组

## Array（数组）对象

```JavaScript
var mycars = new Array("Saab", "Volvo", "BMW"); 
```

> JavaScript数组是动态的。可以添加任意数量的元素。

```JavaScript
var mycars = new Array(); 
mycars[0] = "Saab"; 
mycars[1] = "Volvo"; 
mycars[2] = "BMW"; 
mycars[3] = "Lincoln"; 
```

> 为了更大的简单性、可读性和执行速度，我们可以使用**数组字面量语法**来声明数组。

```JavaScript
var mycars = ["Saab", "Volvo", "BMW"]; 
```

> 尝试访问数组以外的索引，返回值为undefined。

## 数组属性与方法

### length属性

> length属性返回元素的数量。

```JavaScript
var courses = ["HTML", "CSS", "JavaScript"]; 
document.write(courses.length); // -> 3
```

### push()方法

> 使用push()方法在数组末尾增加一个或多个元素：

```JavaScript
var a = []; 
a.push("zero"); // a = ["zero"]
a.push("one", "two"); // a = ["zero", "one", "two"]
```

### pop()方法

> 使用pop()方法删除数组末尾的值**并返回该值**：

```JavaScript
var a = [1, 4, 6]; 
var oneDown = a.pop(); // oneDown = 6, a = [1, 4]
```

### shift()方法

> 使用shift()方法删除数组的第一个值**并返回该值**：

```JavaScript
var a = [1, 4, 6]; 
var oneDown = a.shift(); // oneDown = 1, a = [4, 6]
```

### unshift()方法

> 使用unshift()方法在数组头部增加一个或多个元素：

```JavaScript
var a = []; 
a.unshift("zero"); // a = ["zero"]
a.unshift("one", "two"); // a = ["one", "two", "zero"]
```

### concat()方法

> 使用concat()方法拼接两个数组并返回一个**全新的**数组。【不会影响原数组】

```JavaScript
var c1 = ["HTML", "CSS"]; 
var c2 = ["JS", "Python"]; 
var courses = c1.concat(c2); 
// c1 = ["HTML", "CSS"], c2 = ["JS", "Python"], courses = ["HTML", "CSS", "JS", "Python"]
```

### forEach()方法

> forEach()方法用于调用数组的每个元素，并将元素传递给回调函数。【forEach()对于空数组是不会执行回调函数的】

```JavaScript
var numbers = [64, 45, 72, 11, 49]; 
function myFunction(item, index) {
    demo.innerHTML = demo.innerHTML + "index[" +index + "]: " + item + "<br/>"; 
}
numbers.forEach(myFunction); 
```

### indexOf()方法

> indexOf()方法可返回数组中某个指定元素的第一个位置。若在数组中没有指定元素，则返回-1。

```JavaScript
var fruits = ["banana", "apple", "pineapple", "watermelon", "apple"]; 
var a = fruits.indexOf("apple"); // a = 1
var b = fruits.indexOf("orange"); //b = -1
```

### slice()方法

> slice()方法可从已有数组中返回选定元素， 也可以提取字符串的某个部分，并以新的字符串返回被提取的部分。【slice()方法不会改变原始数组或字符串】
>
> 语法：`array.slice(start, end)`
>
> - 允许输入负值
> - end为空时，直至数组结尾

```JavaScript
var fruits = ["banana", "orange", "lemon", "apple", "mango"]; 
var citrus = fruits.slice(1, 3); // citrus = ["orange", "lemon", "apple"]
```

## 关联数组

> **关联数组**：具有命名索引的数组（文本而不是数字）。
>
> JavaScript**不支持**关联数组，但可以使用命名数组语法产生一个object-array混合体。如：
>
> ```JavaScript
> var person = []; 
> person.name = "Loen"; // 现在person被视为一个object-array混合体，而非普通数组
> person["age"] = 28; 
> document.write(person["name"] + "<br/>"); // -> Loen
> document.write(person.age + "<br/>"); // -> 28
> document.write(person.length + "<br/>"); // -> 0 【当person数组被视为object-array混合体后，标准数组方法和属性将有些变化】
> person[0] = "wang"; // 【特别注意此时person依旧具有数组属性！！！】
> document.write(person[0] + "<br/>"); // -> wang 
> document.write(person[1] + "<br/>"); // -> undefined
> document.write(person["name"] + "<br/>"); // -> Loen
> document.write(person.age + "<br/>"); // -> 28
> document.write(person.length); // -> 1 【即person[0]】
> ```
>
> ```JavaScript
> // 特别注意，我们不能直接实例化一个object-array混合体，只能先创建一个数组或对象后再加入另一个的属性，此时先创建的那个为本体，具有优先级！
> var person_ = {"name": "John", "age": 24, }; 
> document.write("the length of object person_ is " + person_.length + "<br/>"); // -> undefined
> document.write("person_'s name is " + person_.name + "<br/>"); // -> John
> person_[0] = "wang_"; 
> document.write("person_[0] = " + person_[0] + "<br/>"); // -> wang_
> document.write("the length of object person_ now is " + person_.length + "<br/>"); // -> undefined 【特别注意，此处person_本体依旧是对象，故结果仍为undefined！！！】
> ```
>






# JavaScript核心对象

## String对象

> String对象用于处理文本（字符串）。

```JavaScript
var txt = new String("string"); // 即 var txt = "string"; 
```

### String对象方法

\<img src="img/0006.png" alt="0006" style="zoom:50%;" />

![0006](https://i.loli.net/2021/01/31/LG4QSOUzJnKWZro.png)

### JavaScript正则表达式

\![0007]\(img/0007.gif)

![0007](https://i.loli.net/2021/01/31/5abK9rBkfTNCPDp.gif)

## Window对象

> Window对象表示浏览器中打开的窗口。
>
> 如果文档中包含框架（\<frame>或\<iframe>标签），浏览器会为HTML文档创建一个window对象，并为每个框架创建一个额外的window对象。
>
> window作为全局变量，代表了脚本正在运行的窗口，暴露给JavaScript代码。

### Window对象属性

\![0008]\(img/0008.png)

![0008](https://i.loli.net/2021/01/31/ruTjqtxyCgiLcOl.png)

### Windows对象方法

\![0009]\(img/0009.png)

![0009](https://i.loli.net/2021/01/31/TlqSr8ZW6QIRXpY.png)

#### open()方法

> open()方法用于打开一个新的浏览器窗口或查找一个已命名的窗口。
>
> `window.open(URL, name, specs, replace)`
>
> \![0010]\(img/0010.png)
>
> \![0011]\(img/0011.png)
>
> ![0010](https://i.loli.net/2021/01/31/YElpkNuFmD75P8d.png)
>
> ![0011](https://i.loli.net/2021/01/31/T5ARBWrVcKmJXiw.png)
>
> ```JavaScript
> // 在新浏览器窗口中打开www.w3cschool.cn
> function open_win() {
>     window.open("http://www.w3cschool.cn"); 
> }
> ```
>
> ```JavaScript
> // 在新浏览器窗口中打开空白页
> function openWin() {
>     myWindow = window.open("", "", "width=200, height=100"); 
>     myWindow.document.write("<p>It's my window!</p>"); 
>     myWindow.focus(); 
> }
> ```

#### setTimeout()方法

> setTimeout()方法用于在指定的毫秒数后调用函数或计算表达式。【使用clearTimeout()方法来阻止函数的执行。
>
> 如果想重复执行可以使用setInterval()方法；使用clearInterval()方法来阻止函数的执行。

```JavaScript
setTimeout(function(){alert("Hello World!"); }, 3000); 
```

```javascript
var myVar; 

function myFunction() {
    myVar = setTimeout(function(){alert("Hello");}, 3000); 
}

function myStopFunction() {
    clearTimeout(myVar); 
}
```

## JSON

> JSON(**J**ava**S**cript **O**bject **N**otation)是用于存储和传输数据的格式。
>
> JSON通常用于服务端向网页传递数据。
>
> JSON是一种轻量级的数据交换格式。

### JSON实例

```JSON
{"sites": [
    {"name": "W3Cschool", "url": "www.w3cschool.cn"}, 
    {"name": "Google", "url": "www.google.com"}, 
    {"name": "Baidu", "url": "www.baidu.com"}
]}
```

### JSON.parse()方法

> JSON.parse()方法用于将一个JSON字符串转换为对象。
>
> 语法：`JSON.parse(text[, reviver])`
>
> - text：【必需】一个有效的JSON字符串。
> - reviver：【可选】一个转换结果的函数，将为对象的每个成员调用此函数。

```javascript
var text = '{"sites": [
    {"name": "W3Cschool", "url": "www.w3cschool.cn"}, 
    {"name": "Google", "url": "www.google.com"}, 
    {"name": "Baidu", "url": "www.baidu.com"}
]}'; 
obj = JSON.parse(text); 
document.getElementById("demo").innerHTML = obj.sites[1].name + " " + obj.sites[1].url; 
```

```javascript
JSON.parse('{"p": 5, "s": 1.5, "t": -3}', function(k, v){
    if(k === "") return v; // 如果到了最顶层，则直接返回属性值
    return v*2; 
}); // {"p": 10, "s": 3, "t": -6}
```

> 如果带reviver函数遍历属性的顺序是**从内向外**的。

```javascript
JSON.parse('{"1": 1, "2": 2, "3": {"4":4, "5": {"6": 6}}}', function(k, v) {
    console.log(k); // 将属性名输出到控制台
    return v; 
})
// 1 // 2 // 4 // 6 // 5 // 3 // ""
```

> JSON.parse()不允许用逗号作为结尾。

```javascript
JSON.parse("[1, 2, 3, 4, ]"); 
JSON.parse('{"foo": 1, }'); 
```

### JSON.stringify()方法

> JSON.stringify()方法用于将JavaScript值转为JSON字符串。
>
> 语法：`JSON.stringify(value[, replacer[, space]])`
>
> - value：【必需】要转换的JavaScript值（通常为对象或数组）
> - replacer：【可选】用于转换结果的函数或数组。如果replacer为函数，则JSON.stringify将调用该函数，并传入每个成员的键和值。如果该函数返回undefined，则意味着排除该成员。根对象的键是一个空字符串：""。如果replacer是一个数组，则仅转换该数组中具有对应键值的成员。成员的转换顺序与键在数组中的顺序一样。
> - space：【可选】文本添加缩进、空格和换行符，如果space是一个数字，则返回值文本在每个级别缩进指定数目的空格，如果space大于10，则文本缩进10个空格。space也可以使用非数字，如：\t。

```javascript
var str = {"name": "W3Cschool", "site": "http://www.w3cschool.cn"}; 
str_pretty1 = JSON.stringify(str); 
document.write("只有一个参数：<br/><pre>" + str_pretty1 + "</pre><br/>"); 
str_pretty2 = JSON.stringify(str, null, 4)
document.write("使用参数：<br/><pre>" + str_pretty1 + "</pre><br/>"); 
// pre用于格式输出
```

## Math对象

> Math对象提供多种算数值类型和函数。

### Math对象属性

\![0012]\(img/0012.png "Math对象属性")

![0012](https://i.loli.net/2021/02/01/Qt1H5iRZj2bczIh.png "Math对象属性")

### Math对象方法

\![0013]\(img/0013.png "Math对象方法")

![0013](https://i.loli.net/2021/02/01/iYRpWOV69M2lykj.png "Math对象方法")

> 注意：与很多其他语言中的round()函数不同的是，Math.round()并不总是舍到远离0的方向，如：`x = Math.round(-20.5); //-20`。

## 时间对象

### setInterval()方法

> setInterval()方法调用函数或以指定的间隔（以毫秒为单位）来计算表达式。
>
> 它将持续调用该函数，直到调用clearInterval()或窗口关闭。

```javascript
function myAlert() {
    alert("Hello World!"); 
}
setInterval(myAlert, 3000); //每隔3秒执行一次myAlert
```

### Date对象

> 日期由**年、月、日、时、分、秒和毫秒**组成。
>
> 使用new Date()，将创建一个存储当前日期和时间的日期对象。

```javascript
var d = new Date(); // d 存储了当前的日期和时间
```

> 初始化日期的其他方法允许从指定的日期和时间创建新的日期对象。
>
> JavaScript日期以**1970年01月01日00:00:00**世界时（UTC）计算。一天包含**86400000**毫秒。
>
> JavaScript计数**从0到11，依次代表1月到12月**。

```javascript
new Date(milliseconds); // 毫秒
// Fri Jan 02 1970 08:00:00 GMT+0800 (中国标准时间)
var d1 = new Date(86400000); 

new Date(dateString); // 日期字符串
// Thu Oct 19 2017 15:56:00 GMT+0800 (中国标准时间)
var d2 = new Date("October 19, 2017 15:56:00"); 

new Date(year, month, day, hours, minutes, seconds, milliseconds); // 年, 月, 日, 时, 分, 秒, 毫秒
// Sat Jun 11 1988 11:42:00 GMT+0800 (中国标准时间)
var d3 = new Date(88, 5, 11, 11, 42, 00); 
```

### Date方法

\![0014]\(img/0014.png "Date方法")

\![0015]\(img/0015.png "Date方法")

\![0016]\(img/0016.png "Date方法")

![0014](https://i.loli.net/2021/02/01/sv7OYZwQA1N3eHB.png "Date方法")

![0015](https://i.loli.net/2021/02/01/b9SvUjmMdW2AcQ4.png "Date方法")

![0016](https://i.loli.net/2021/02/01/GA1HU5WvBwcP8Ra.png "Date方法")








# DOM

## 动画

```html
<style>
    #container {
        width: 200px; 
        height: 200px; 
        background: green; 
        position: relative; 
    }
    #box {
        width: 30px; 
        height: 30px; 
        background: red; 
        position: absolute; 
    }
    /* 容器是相对的，盒子是绝对的。
    这将允许我们创建相对于容器的动画。 */
</style>
<div id="container">
    <div id="box"></div>
</div>
```

<div style="width: 200px; height: 200px; background: green; position: relative; "><div style="width: 30px; height: 30px; background: red; position: absolute; "></div></div>

```javascript
// 定义开始的位置
var pos = 0; 
// 获取box元素
var box = document.getElementById("box"); 
// 使用setInterval()方法反复调用move()函数
var t = setInterval(move, 10); 
// 定义一个move()函数，以改变框的位置
function move() {
    if (pos >= 170) {
        clearInterval(t); 
    }
    else {
    	pos += 1; 
    	box.style.left = pos + "px"; 
	}
}
```

## DOM

> 通过HTML DOM，JavaScript可以访问HTML文档的所有元素。
>
> 当网页被加载时，浏览器会创建页面的文档对象模型（**D**ocument **O**bject **M**odel），HTML DOM模型被构造为对象的树：【\<html>有两个子节点\<head>和\<body>，后两者互为兄弟节点】
>
> \<img src="img/0017.png" alt="0017" style="zoom:50%;" />
>
> <img src="https://i.loli.net/2021/02/01/ctwaU5h9Jr2EIBA.png" alt="0017" style="zoom:50%;" />
>
> 通过可编程的对象模型，JavaScript获得了足够的能力来创建动态的HTML
>
> - JavaScript能改变页面中的所有HTML元素
> - JavaScript能改变页面中的所有HTML属性
> - JavaScript能改变页面中的所有CSS样式
> - JavaScript能对页面中的所有事件做出反应

## 选择元素

> document对象有三种方法最常用于选择HTML元素：

```javascript
// 通过 id 找元素，返回单一元素
document.getElementById(id)
// 通过 类 找元素，返回数组
document.getElementByClassName(name)
// 通过 标签 找元素，返回数组
document.getElementByTagName(name)
```

> DOM中的每个元素都有一组属性和方法，它们提供有关它们在DOM中的关系的信息：
>
> - element.childNodes：返回一个元素的子节点的数组
> - element.firstChild：返回元素的第一个子节点
> - element.lastChild：返回元素的最后一个子节点
> - element.hasChildNodes：如果元素有任何子节点，则返回true，否则为false
> - element.nextSibling：返回相同树级别的下一个兄弟节点
> - element.previousSibling：返回相同树级别的上一个兄弟节点
> - element.parentNode：返回元素的父节点

```html
<html>
    <body>
        <div id="demo">
            <p>
                some text
            </p>
            <p>
                another text
            </p>
        </div>
        <script>
        	var a = document.getElementById("demo"); 
            var arr = a.childNodes; 
            for (var x = 0; x < arr.length; x++) {
                arr[x].innerHTML = "new text"; 
            }
        </script>
    </body>
</html>
```

## 改变属性

> JavaScript可以更改元素的所有属性。

```html
<!-- 更改图像的src属性 -->
<img id="myImg" src="https://www.w3cschool.cn/attachments/cover/cover_php.jpg" alt="" />
<script>
	var el = document.getElementById("myImg"); 
    el.src = "https://www.w3cschool.cn/attachments/cover/cover_html.png"; 
</script>
```

```html
<!-- 更改链接的href属性 -->
<a href="http://www.baidu.com">百度</a>
<script>
	var el = document.getElementByTagName("a"); 
    el[0].href = "https://www.w3cschool.cn"; 
    el[0].innerHTML = "W3Cschool"; 
</script>
```

> 可以使用元素的style对象来访问所有的样式属性。【特别注意：我们不能在属性名称中使用破折号（-），应用驼峰写法来替换。如：background-color应换为backgroundColor】

```html
<div id="demo" style="width: 200px">
    some text
</div>
<script>
	var x = document.getElementById("demo"); 
    x.style.color = "#6600ff"; 
    x.style.width = "100px"; 
</script>
```

## 添加和移除元素

> 使用以下方法创建新节点：
>
> - element.cloneNode()：克隆元素并返回结果节点
> - document.createElement(element)：创建一个新的元素节点
> - document.createTextNode(text)：创建一个新的文本节点【如：`var node = document.createTextNode("some new text"); `，但它不会出现在文档中，直到我们使用如下方法将其附加到现有元素：
>   - element.appendChild(newNode)将一个新的子节点添加到元素作为最后一个子节点
>   - element.insertBefore(node1, node2)在节点2之前插入节点1作为element的子节点

```html
<div id="demo">
    some text
</div>
<script>
	// create a paraagraph
    var p = document.createElement("p"); 
    var node = document.createTextNode("another text"); 
    // append node to p
    p.appendChild(node); 
    
    var div = document.getElementById("demo"); 
    // append p to div
    div.appendChild(p); 
</script>
```

> 要移除HTML元素，必须选择元素的父节点并使用removeChild(node)方法。

```html
<div id="demo">
    <p id="p1">
        a paragraph
    </p>
    <p id="p2">
        another paragraph
    </p>
</div>
<script>
	var parent = document.getElementById("demo"); 
    var child = document.getElementById("p1"); 
    parent.removeChild(child); 
    /* 或者使用如下方法 
    var child = document.getElementById("p1"); 
    child.parentNode.removeChild(child); */
</script>
```

> 要替换HTML元素，使用element.replaceChild(newNode, oldNode)方法。

```html
<div id="demo">
    <p id="p1">
        a paragraph
    </p>
    <p id="p2">
        another paragraph
    </p>
</div>
<script>
	var p = document.createElement("p"); 
    var node = document.createTextNode("new paragraph"); 
    p.appendChild(node); 
    
    var parent = document.getElementById("demo"); 
    var child = document.getElementById("p1"); 
    parent.replaceChild(p, child); 
</script>
```





# JavaScript事件

## 事件

> **事件流**：事件的轨迹，一般分为三个阶段：捕获阶段、目标阶段、冒泡阶段。

\![0018]\(img/0018.png "完整事件流")

![0018](https://i.loli.net/2021/02/01/uxX52IFRpHQ1Mds.png "完整事件流")

> 常见的HTML事件如下：【相应的事件可以添加到HTML元素作为属性】

\![0019]\(img/0019.png "常见的HTML事件")

![0019](https://i.loli.net/2021/02/01/6I4CQU5FuiTkPXq.png "常见的HTML事件")

### 处理事件

```html
<button onclick="show()">
    click!
</button>
<script>
    function show() {
		alert("Hello foolish!"); 
    }
</script>
```

> 可以给元素绑定事件监听

```javascript
var x = document.getElementById("demo"); 
x.onclick = function() {
    document.getElementById("date").innerHTML = new Date(); 
}
```

### 事件监听

> addEventListener()方法将事件处理程序附加到元素，而不会覆盖现有的事件处理程序。
>
> 我们还可以将许多同一类型的事件处理程序添加到一个元素。
>
> `element.addEventListener(event, function[, useCapture]); `
>
> - useCapture【布尔值】指定是否使用事件冒泡或事件捕获。【可选【
>
> 注意：在添加事件类型的时候没有on，用的是click而非onclick。

### 删除事件监听

> 使用removeEventListener()方法删除事件监听。

```html
<button id="demo">
    start
</button>
<script>
	var btn = document.getElementById("demo"); 
    btn.addEventListener("click", myFunction); 
    
    function myFunction() {
		alert(Math.random()); 
        btn.removeEventListener("click", myFunction); 
    }
</script>
```

## 图像幻灯片-实例

```html
<div>
    <button onclick="last()">last</button>
    <img id="slider" src="https://www.w3cschool.cn/statics/images/logo.png" />
    <button onclick="next()">next</button>
</div>
<script>
	var images = [
        "https://sm.ms/image/LhYQsUGgPcfNI3b", 
        "https://sm.ms/image/72fin4FSjDYr3G9", 
        "https://sm.ms/image/aKR2LzoXCVF6Nnp", 
        "https://sm.ms/image/ha7iHEvYMIgU3Wc", 
        "https://sm.ms/image/ARl6wdHCDU59tgz", 
        "https://sm.ms/image/tMV7IfRnQ9aO4su"
    ]
    var num = 0; 
    function last() {
        var slider = document.getElementById("slider"); 
        num--; 
        if (num < 0) {
            num = images.length - 1; 
        }
        slider.src = images[num]; 
    }
    function next() {
        var slider = document.getElementById("slider"); 
        num++; 
        if (num >= images.length) {
            num = 0; 
        }
        slider.src = images[num]; 
    }
</script>
```

## 表格验证

> 表单元素具有可以处理以执行验证的onsubmit事件。【当onsubmit事件返回false时，表单将不会被提交。

```html
<form onsubmit="return validate()" method="post">
    String: <input type="text" name="text1" id="text1" /><br/>
    Repeat: <input type="text" name="text2" id="text2" /><br/>
    <input type="submit" value="confirm" />
</form>
<script>
	function validate() {
        var t1 = document.getElementById("text1"); 
        var t2 = document.getElementById("text2"); 
        if (t1.value != "" && t2.value != "") {
            if (t1.value == t2.value) {
                return true; 
            }
        }
        alert("输入的两个值不相等，要重新输入~"); 
        return false; 
    }
</script>
```




