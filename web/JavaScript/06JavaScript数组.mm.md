# JavaScript数组

## Array（数组）对象

```JavaScript
var mycars = new Array("Saab", "Volvo", "BMW"); 
```

> JavaScript数组是动态的。可以添加任意数量的元素。

```JavaScript
var mycars = new Array(); 
mycars[0] = "Saab"; 
mycars[1] = "Volvo"; 
mycars[2] = "BMW"; 
mycars[3] = "Lincoln"; 
```

> 为了更大的简单性、可读性和执行速度，我们可以使用**数组字面量语法**来声明数组。

```JavaScript
var mycars = ["Saab", "Volvo", "BMW"]; 
```

> 尝试访问数组以外的索引，返回值为undefined。

## 数组属性与方法

### length属性

> length属性返回元素的数量。

```JavaScript
var courses = ["HTML", "CSS", "JavaScript"]; 
document.write(courses.length); // -> 3
```

### push()方法

> 使用push()方法在数组末尾增加一个或多个元素：

```JavaScript
var a = []; 
a.push("zero"); // a = ["zero"]
a.push("one", "two"); // a = ["zero", "one", "two"]
```

### pop()方法

> 使用pop()方法删除数组末尾的值**并返回该值**：

```JavaScript
var a = [1, 4, 6]; 
var oneDown = a.pop(); // oneDown = 6, a = [1, 4]
```

### shift()方法

> 使用shift()方法删除数组的第一个值**并返回该值**：

```JavaScript
var a = [1, 4, 6]; 
var oneDown = a.shift(); // oneDown = 1, a = [4, 6]
```

### unshift()方法

> 使用unshift()方法在数组头部增加一个或多个元素：

```JavaScript
var a = []; 
a.unshift("zero"); // a = ["zero"]
a.unshift("one", "two"); // a = ["one", "two", "zero"]
```

### concat()方法

> 使用concat()方法拼接两个数组并返回一个**全新的**数组。【不会影响原数组】

```JavaScript
var c1 = ["HTML", "CSS"]; 
var c2 = ["JS", "Python"]; 
var courses = c1.concat(c2); 
// c1 = ["HTML", "CSS"], c2 = ["JS", "Python"], courses = ["HTML", "CSS", "JS", "Python"]
```

### forEach()方法

> forEach()方法用于调用数组的每个元素，并将元素传递给回调函数。【forEach()对于空数组是不会执行回调函数的】

```JavaScript
var numbers = [64, 45, 72, 11, 49]; 
function myFunction(item, index) {
    demo.innerHTML = demo.innerHTML + "index[" +index + "]: " + item + "<br/>"; 
}
numbers.forEach(myFunction); 
```

### indexOf()方法

> indexOf()方法可返回数组中某个指定元素的第一个位置。若在数组中没有指定元素，则返回-1。

```JavaScript
var fruits = ["banana", "apple", "pineapple", "watermelon", "apple"]; 
var a = fruits.indexOf("apple"); // a = 1
var b = fruits.indexOf("orange"); //b = -1
```

### slice()方法

> slice()方法可从已有数组中返回选定元素， 也可以提取字符串的某个部分，并以新的字符串返回被提取的部分。【slice()方法不会改变原始数组或字符串】
>
> 语法：`array.slice(start, end)`
>
> - 允许输入负值
> - end为空时，直至数组结尾

```JavaScript
var fruits = ["banana", "orange", "lemon", "apple", "mango"]; 
var citrus = fruits.slice(1, 3); // citrus = ["orange", "lemon", "apple"]
```

## 关联数组

> **关联数组**：具有命名索引的数组（文本而不是数字）。
>
> JavaScript**不支持**关联数组，但可以使用命名数组语法产生一个object-array混合体。如：
>
> ```JavaScript
> var person = []; 
> person.name = "Loen"; // 现在person被视为一个object-array混合体，而非普通数组
> person["age"] = 28; 
> document.write(person["name"] + "<br/>"); // -> Loen
> document.write(person.age + "<br/>"); // -> 28
> document.write(person.length + "<br/>"); // -> 0 【当person数组被视为object-array混合体后，标准数组方法和属性将有些变化】
> person[0] = "wang"; // 【特别注意此时person依旧具有数组属性！！！】
> document.write(person[0] + "<br/>"); // -> wang 
> document.write(person[1] + "<br/>"); // -> undefined
> document.write(person["name"] + "<br/>"); // -> Loen
> document.write(person.age + "<br/>"); // -> 28
> document.write(person.length); // -> 1 【即person[0]】
> ```
>
> ```JavaScript
> // 特别注意，我们不能直接实例化一个object-array混合体，只能先创建一个数组或对象后再加入另一个的属性，此时先创建的那个为本体，具有优先级！
> var person_ = {"name": "John", "age": 24, }; 
> document.write("the length of object person_ is " + person_.length + "<br/>"); // -> undefined
> document.write("person_'s name is " + person_.name + "<br/>"); // -> John
> person_[0] = "wang_"; 
> document.write("person_[0] = " + person_[0] + "<br/>"); // -> wang_
> document.write("the length of object person_ now is " + person_.length + "<br/>"); // -> undefined 【特别注意，此处person_本体依旧是对象，故结果仍为undefined！！！】
> ```
>