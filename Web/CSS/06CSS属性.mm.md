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

