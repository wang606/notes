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

