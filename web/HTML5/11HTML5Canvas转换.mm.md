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

