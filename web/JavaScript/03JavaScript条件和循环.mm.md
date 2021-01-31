# JavaScript条件和循环

### if-else if-else语句

```javascript
if (条件01) {
    // 条件01为true时会执行的代码 
}
else if (条件02) {
    // 条件01位false且条件02位true时会执行的代码
}
else {
    // 条件01和条件02都为flase时会执行的代码
}
```

### switch语句

```JavaScript
switch(表达式) {
    case 结果1:
        // 表达式==结果1时会执行的代码
        break; 
    case 结果2:
        // 表达式==结果2时会执行的代码
        break; 
    ...
    case 结果n:
        // 表达式==结果n时会执行的代码
        break; 
    default:
        // 表达式与上述所有结果不等时会执行的代码
}
```

### for循环

```JavaScript
/*
Statement01：在循环开始前执行； 
Statement02：定义运行循环的条件； 
Statement03：在执行循环后都会执行； 
*/
for (Statement01; Statement02; Statement03) {
    // 循环执行的代码
}
```

### while循环

```JavaScript
while (条件) {
    // 只要“条件”为true就会执行的代码
}
```

### do while循环

```JavaScript
do {
    // 有可能被循环执行的代码（当“条件”为true时）
}
while (条件); 
```

### break与continue语句

> break语句用于跳出当前循环； 
>
> continue语句跳出循环后会继续执行循环之后的代码； 

### JS标签

> JavaScript允许语句前面设置标签（label）相当于定位符，用于跳转到程序的任意位置。
>
> `label: 语句`标签可以是任意非保留字的标识符，语句部分可以是任意语句。

> 标签通常与break语句和continue语句配合使用，跳出特定的循环。

```JavaScript
// 跳出双层循环
label01: for (var i = 0; i < 3; i++) {
    for (var j = 0; j < 3; j++) {
        if (i === 1 && j === 1) break label01; 
        console.log("i=" + i + ", j=" + j + "; "); 
    }
}// i=0, j=0; i=0, j=1; i=0, j=2; i=1, j=0; 
```

```JavaScript
// 跳出区块
label02: {
    console.log("本行正常输出"); 
    break label02; 
    console.log("本行不会输出"); 
}
console.log("本行也正常输出"); 
```



