---
title: 三个实用的javascript小技巧
author: leandrosimoes
author_link: https://github.com/leandrosimoes 
tags:
    - js
---

从后向前获取数组元素
如果你想从后向前获取一个数组的元素，可以这样写：
```js
var newArray = [1, 2, 3, 4]

console.log(newArray.slice(-1)) // [4]
console.log(newArray.slice(-2)) // [3, 4]
console.log(newArray.slice(-3)) // [2, 3, 4]
console.log(newArray.slice(-4)) // [1, 2, 3, 4]
```

短路条件句
如果你想在某个条件逻辑值为true时，执行某个函数，就像这样：

```js
if (condition) {
  dosomething()
}
```

这时，你可以这样子运用短路：

```js
condition && dosomething()
```

用操作符 “||” 来设置默认值
如果你必须给一个变量赋默认值，可以简单的这样写：

```js
var a

console.log(a) // undefined

a = a || 'default value'

console.log(a) // default value

a = a || 'new value'

console.log(a) // default value
```