# HTML5地理定位

> Geolocation API用于获取用户的地理位置，其主要方法是getCurrentPosition。

```html
<div id="demo"></div>
<script>
	var x=document.getElementById("demo");
    function getLocation(){
        if (navigator.geolocation){
            navigaor.geolocation.getCurrentPosition(showPosition);
        }
        else{
            x.innerHTML="your browser doesn't support Geolocation!";
        }
    }
    function showPosition(position){
        x.innerHTML="latitude: " + position.coords.latitude + "<br/>longitude: " + position.coords.longitude;
    }
</script>
```

### 百度API

```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8" />
        <title>baiduAPI</title>
		<!-- 引入百度API，ak是密钥，可以自己申请。 -->
        <script type="text/javascript" src="https://api.map.baidu.com/api?v=2.0&ak=7a6QKaIilZftIMmKGAFLG7QT1GLfIncg"></script>
    </head>
    <body> 
        <input type="button" onclick="getLocation()" value="定位" />
        <div id="position"></div>
        <script type="text/javascript">
        	var x=document.getElementById("position");
            function getLocation(){
                //创建百度API位置实例，代替navigator.geolaocation
                var geolocation=new BMap.Geolocation();
                geolocation.getCurrentPosition(function(e) {
                    if (this.getStatus() == BMAP_STATUS_SUCCESS){
                        x.innerHTML="纬度：" + e.point.lat + "<br/>经度：" + e.point.lng;
                    }
                    else {
                        x.innerHTML="failed" + this.getStatus();
                    }
                });
            }
        </script>
    </body>
</html>
```

