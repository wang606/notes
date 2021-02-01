# JavaScript函数

### 函数定义

```JavaScript
function functionName(parameters) {
    // 函数中的代码
}
```

### 函数参数

> 函数显式参数在函数定义时列出，函数隐式参数arguments是函数调用时传递给函数真正的值。如
>
> ```JavaScript
> function sum() {
>  return arguments[0] + arguments[1]; 
> }
> sum(1, 2); //3
> ```
>
> 参数规则：
>
> - JavaScript函数定义时参数没有指定数据类型；
> - JavaScript函数对隐藏参数（arguments）没有进行检测；
> - JavaScript函数对隐藏参数（arguments）的个数没有进行检测。
>
> 多参数用逗号“, ”分隔，调用函数时如果缺少参数，则缺少值为undefined。

### 变量作用域

> **作用域**是可访问变量的集合。【在JavaScript中，**对象**和**函数**同样是变量】
>
> JavaScript局部作用域：
>
> - 变量在函数内声明，变量为局部作用域，局部变量只能在函数内部访问。
> - 局部变量在函数开始执行时创建，函数执行完后局部变量会自动销毁。
> - 局部变量的优先级高于同名的全局变量。
>
> JavaScript全局变量：
>
> - 变量在函数外定义即全局变量，全局变量网页中所有脚本和函数均可使用。
>
> - <span style="color: #800000">如果变量在函数内没有声明（没有使用var关键字），则该变量为全局变量。</span>如：
>
>   ```JavaScript
>   // 此处可调用carName变量
>   
>   function myFunction() {
>       carName = "大众"; 
>       // 此处carName为全局变量！
>   }
>   ```
>
> - 全局变量在页面关闭后销毁。
>
> HTML中的全局变量：
>
> - 在HTML中，全局变量是**window**对象：**所有数据变量都属于window对象**。
>
>   ```JavaScript
>   // 此处可用window.carName
>   
>   function myFunction() {
>       carName = "大众"; 
>   }
>   ```

### 弹出框

> JavaScript提供三种类型的弹出框：
>
> - Alert
> - Prompt
> - Confirm

#### Alert警告框

> 当弹出警告框时，用户必须单击“确定”以继续。
>
> 警报功能采用单个参数，即弹出框中显示的文本。
>
> 使用alert弹出框，将阻塞整个页面的运行，点击确定后才继续运行。

```JavaScript
alert("Hello World!"); 
```

\![0003]\(img/0003.png)

![0003](https://i.loli.net/2021/01/31/LpGtYjkcKOSdNr9.png)

#### Prompt框

> 通常使用Prompt框来让用户输入一个值。
>
> 当弹出提示框（Prompt框）时，输入输入值后，用户将不得不单击“确定”或“取消”以继续。
>
> 如果用户单击确定，该框将返回输入值；如果用户单击取消，该框将返回null。
>
> Prompt()方法有两个参数：
>
> - 第一个是要在文本框中显示的标签
> - 第二个是在文本框中显示的默认字符串【可选】

```JavaScript
var input = prompt("so embarrassed, em...ok, input something: ", "Hurry up!"); 
alert(input); 
```

\![0004]\(img/0004.png)

![0004](https://i.loli.net/2021/01/31/5sUpaViSQnywY6q.png)

#### Confirm框

> 通常使用Confirm框让用户验证或接受某些内容。
>
> 当弹出确认框（Confirm框）时，用户必须单击“确定”或“取消”以继续。
>
> 如果用户单击确定，该框将返回true；如果用户单击取消，该框将返回false。

```JavaScript
var result = confirm("Are you sure to leave?"); 
if (result === true) {
    alert("get away!"); 
}
else {
    alert("I have bet it!"); 
}
```

\![0005]\(img/0005.png)

![0005](https://i.loli.net/2021/01/31/gitsyVXBTJWUnlI.png)