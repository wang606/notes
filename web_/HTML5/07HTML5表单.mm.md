# HTML5表单

### placeholder属性

> placeholder属性在\<input>和\<textarea>元素上提供提示，描述输入域所期待的值。提示在用户输入之前会显示在输入域上。

```html
<form>
    <input type="text" name="firstname" placeholder="First name"><br/>
    <input type="text" name="lastname" placeholder="Last name"><br/>
    <input type="submit" value="Confirm">
</form> 
```

### autofocus属性

> autofocus属性规定在页面添加加载时，域自动地获得焦点。

```html
<form>
    <input type="text" name="firstname" placeholder="First name autofocus"><br/>
    <input type="text" name="lastname" placeholder="Last name"><br/>
    <input type="submit" value="Confirm">
</form> 
```

### required属性

> required属性规定必须在提交之前填写输入域（不能为空）。

```html
<form autocomplete="off">
    Username: <input type="text" name="username" required>
    <input type="submit">
</form>
```

> autocomplete属性规定form或input域应该拥有自动完成功能。当用户在自动完成域中开始输入时，浏览器应该在该域或中显示填写的选项。

### search类型

> search类型可用于创建搜索框。

```html
<input type="search" name="searchitem">
```

### \<datalist>

> \<datalist>元素规定输入域的选项列表。

```html
<input list="browsers">
<datalist id="browsers">
	<option value="Internet Explorer"></option>
    <option value="Firefox"></option>
    <option value="Chrome"></option>
    <option value="Opera"></option>
    <option value="Safari"></option>
</datalist>
```

### 更多的输入类型

> email、tel、url、date、time等。

```html
<form>
    <input type="email" name="email" placeholder="example@example.com"><br/>
    <input type="tel" name="tel" placeholder="000.000.0000"><br/>
    <input type="url" name="homepage" placeholder="example.com">
</form>
```

