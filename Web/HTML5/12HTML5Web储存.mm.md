# HTML5Web存储

> 在HTML5之前，本地存储使用的是cookie。
>
> Web存储的优势：
>
> - 更加安全
> - 更加快速
> - 可以存储大量的数据
> - 每个服务器请求都不会发送存储的数据
>
> 数据以 键/值 对存在，Web网页的数据只允许该网页访问使用。

> Web储存对象有两种类型：
>
> - localStorage：存储的数据没有时间限制。
> - sessionStorage：针对一个session进行数据存储。当用户关闭浏览器窗口后，数据会被删除。

> Web存储使用的API：
>
> - 保存数据：
>
>   localStorage.setItem(key, value);
>
> - 读取数据：
>
>   localStorage.getItem(key);
>
> - 删除单个数据：
>
>   localStorage.removeItem(key);
>
> - 清除所有数据：
>
>   localStorage.clear();
>
> - 得到某个索引的key:
>
>   localStorage.key(index);

