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

