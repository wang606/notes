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

