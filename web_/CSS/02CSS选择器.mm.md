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

