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

