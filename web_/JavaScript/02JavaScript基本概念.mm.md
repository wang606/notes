# JavaScript基本概念

### 语句

> 语句（statement）是为了完成某种任务而进行的操作。
>
> 语句以分号结尾。

### 变量

> 变量是用于存储信息的容器，变量的值可以在整个程序中被修改。
>
> 变量使用关键字var来声明， 初始值为undefined。
>
> JavaScript区分大小写。 

> typeof运算符用来监测一个变量的类型，返回一个字符串。

#### 变量提升

> JavaScript引擎先解析代码，获取所有被声明的变量，然后再一行行地运行。也就是说，所有变量的声明语句都会被提升到代码的头部， 这就叫做**变量提升（hoisting）**。

> `console.log(a); var a = 1; `不会报错， 但真正运行的是`var a; console.log(a); a = 1; `，最后的结果是显示undefined！

### 区块

> JavaScript使用大括号将多个相关语句组合在一起，称为区块（block）。
>
> 对于var命令来说，JavaScript的区块不构成单独的作用域（scope）。如`{var a = 1; } document.write(a); // 1`中var在区块内，但在区块外依然有效。

### 数据类型

> JavaScript有五种数据类型：
>
> - 字符串（string）
> - 数字（number）
> - 布尔（boolean）
> - 空（null）
> - 未定义（undefined）
> - 对象（object）
> - symbol

#### null与undefined

> null是一个表示“空”的对象（typeof null == object），转为数值时为0； 
>
> undefined是一个表示“此处无定义”的原始值（typeof undefined == undefined），转为数值时为NaN。

#### boolean

> 下列运算符会返回布尔值：
>
> - 两元逻辑运算符：&&(And), ||(Or)
> - 前置逻辑运算符：!(Not)
> - 相等运算符：===, !==, ==, !=
> - 比较运算符：>, >=, <, <=
>
> 若JavaScript预期某个位置应该是布尔值，则会自动将值转为布尔值。转换规则是除下列六个值被转为false外，其他值都视为true【特别注意空数组（[]）和空对象（{}）对应布尔值为true】：
>
> - undefined
> - null
> - false
> - 0
> - NaN
> - ""或''（空字符串）

#### number

> JavaScript只有一种数值类型，数值可以带小数点也可不带。

#### string

> 字符串用双引号""或单引号''包裹。
>
> 用反斜杠\转义。

### 三元运算符

> `(条件) ? 表达式1 : 表达式2`如果“条件”为true则返回“表达式1”的值， 否则返回“表达式2”的值。

### 比较运算符

给定x=5，有如下结果：

\![0001]\(img/0001.jpg)

![0001](https://i.loli.net/2021/01/30/FSOvQ7KVI2oyXY8.jpg)

### 赋值运算符

\![0002]]\(img/0002.jpg)

![0002](https://i.loli.net/2021/01/30/6h3al5tsgWmOSRL.jpg)

### 字符串

> 字符串是可检索的。

>  特殊字符
>
> - \n：换行
> - \r：回车
> - \t：tab（制表符）
> - \b：退格符
> - \f：换页符

> 使用length来计算字符串长度。

> 字符串运算符：
>
> +符号连接字符串

> 字符串的不变性：
>
> JavaScript中字符串一旦被创建就不能被修改。