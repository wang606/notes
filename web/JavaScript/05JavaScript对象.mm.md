# JavaScript对象

> JavaScript对象是拥有属性和方法的数据。
>
> JavaScript中的一切皆对象：字符串、数值、数组、函数....此外，JavaScript也允许自定义对象。

### 对象定义

```JavaScript
var myObject = {
    name01: value01, name02: value02, ...
}
```

> 其中，myObject即对象，name为对象的属性，value为对象属性对应的值。如：

```JavaScript
var person = {
    name: "John", age: 31, favColor: "green", height: 183, 
}; 
```

### 对象属性

> 可以通过`objectName.propertyName`或`objectName["propertyName"]`访问对象属性。

### 对象构造器

```JavaScript
function person(firstname, lastname, age, eyecolor) {
    this.firstname = firstname; 
    this.lastname = lastname; 
    this.age = age; 
    this.eyecolor = eyecolor; 
}
```

> this通常指向我们正在执行的函数本身，或该函数所属的对象。

#### 创建JavaScript对象实例

```JavaScript
var myFather = new person("John", "Doe", 50, "blue"); 
var myMother = new person("Sally", "Rally", 48, "green"); 
```

### 对象初始化

> 使用英文大括号{}创建**单个**对象：
>
> ```JavaScript
> var John = {name: "John", age: 25}; 
> var Loen = {name: "Loen", age: 28};  
> ```

### 添加方法

> 方法是存储在对象属性中的函数。
>
> 创建对象函数：`methodName: function(paraments) { code lines }`; 
>
> 使用`objectName.methodName()`访问对象函数。

```JavaScript
function person(name, age) {
    this.name = name; 
    this.age = age; 
    this.changeName = function (name) {
        this.name = name; 
    }
}

var p = new person("Loen", 28); 
p.changeName("John"); 
```

> 我们也可以在构造函数外定义一个函数，通过函数名关联到对象的属性上：【注意将函数关联到对象属性时不需要写括号】

```JavaScript
function person(name, age) {
    this.name = name; 
    this.age = age; 
    this.yearOfBirth = bornYear; // 关联到bornYear函数
}
function bornYear() {
    return new Date().getFullYear() - this.age; 
}
```

