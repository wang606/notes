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

