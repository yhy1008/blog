title: js一些常用函数
author: yhy
tags:
  - js
categories:
  - 前端
date: 2020-11-11 16:35:00
---
### filter
filter() 方法创建一个新的数组，新数组中的元素是通过检查指定数组中符合条件的所有元素。  
注意：   
filter() 不会对空数组进行检测。  
filter() 不会改变原始数组。    
**语法：**
array.filter(function(currentValue,index,arr), thisValue)
### map
map() 方法返回一个新数组，数组中的元素为原始数组元素调用函数处理后的值。  
注意：   
map() 不会对空数组进行检测。  
map() 不会改变原始数组。  
**语法：**
array.map(function(currentValue,index,arr), thisValue)
* 描述  
currentValue	必须。当前元素的值  
index	可选。当前元素的索引值  
arr	可选。当前元素属于的数组对象

### concat
concat() 方法用于合并两个或多个数组。此方法不会更改现有数组，而是返回一个新数组。   
注意：   
concat() 不会改变原始数组。  
如果省略了valueN参数，则concat会返回old_array数组的浅拷贝。  
**语法：**
var new_array = old_array.concat(value1[, value2[, ...[, valueN]]])

### reverse
reverse() 方法用于颠倒数组中元素的顺序。返回的是颠倒后的数组，会改变原数组。  
```
var arr = [1,2,3];
console.log(arr.reverse()); //[3, 2, 1]
console.log(arr);  //[3, 2, 1]
```
注意：   
reverse() 会改变原数组。

### every与some
every与some两个方法是判读数组中每一项满不满足这个条件。  
every表示每一项都满足返回true，否则返回false。  
some表示数组中有满足的就返回true，否则false。
```
var arr = [1,2,3]
var res = arr.every(function(item,index){
	return item > 2
})
console.log(res) // false
var res = arr.some(function(item,index){
	return item > 2
})
console.log(res) // true
```
### set
set() 方法用来去重数组。 
```
var mySet = new Set([1, 2, 2, 3]);
let newArr = Array.from(mySet);
console.log(newArr); // [1, 2, 3]
```
>展开操作符 …(点点点)

`[...mySet]; // [1, 2, 3]`

### flat
flat()方法处理嵌套数组转一维数组。  
flat(depth)，参数depth，代表展开嵌套数组的深度，默认是1
```
let arr = [1, [2, 3, [4, [5]]]];
arr.flat(3); // [1,2,3,4,5]
```

### 箭头函数
>箭头函数是ES6标准新增的一种函数，简化了函数定义。

**箭头函数：**
x => x * x  
上面的箭头函数相当于：
```
function (x) {
    return x * x;
}
```
注意：  
箭头函数有两种格式，一种像上面的，只包含一个表达式，连{}和return都省略掉了。还有一种可以包含多条语句，这时候就不能省略{}和return：
```
arr.map((x, y) => {
    return ???
});
```