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



