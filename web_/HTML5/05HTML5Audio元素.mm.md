# HTML5 Audio元素

> \<audio>标签定义声音，比如**音乐或其他音频流**。目前，\<audio>元素支持3种文件格式：MP3、Wav、Ogg。

```html
<audio controls>
	<source src="https://www/w3cschool.cn/statics/demosource/horse.mp3" type="audio/ogg">
    <source src="https://www/w3cschool.cn/statics/demosource/horse.ogg" type="audio/mpeg">
    your browser doesn't support audio!
</audio>
```

> \<source>标签用来定义多种媒体资源，\<control>属性供添加播放、暂停和音量控件。
>
> \<audio>元素允许使用多个\<source>以链接不同的音频文件，浏览器将使用第一个支持的音频文件。
>
> \<audio>与\</audio>之间的文字将在不支持\<audio>标签的浏览器上显示。

> src属性规定音频文件的URL。
>
> autoplay属性让音频在就绪后马上播放。
>
> loop属性让音频结束时重新开始播放。