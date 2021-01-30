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

