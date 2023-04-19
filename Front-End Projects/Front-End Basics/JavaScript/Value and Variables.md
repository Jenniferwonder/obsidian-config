---
title: Value and Variables
tags: JS
started: 2022-12-02 Fri
due:
modified: 2022-12-15 Thu
status:
---

>[Storing the information you need — Variables - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Variables)
## Value and Variable
#### 1. Value
- [[Data Types and Data Structures#Primitive Data Type]]
#### 2. Variable
- Dynamic Data Type
- A container that stores value
## Three ways to declare variables
>[[Scope-作用域]]
1. `var` 定义的变量，没有块的概念，可以跨块访问, 可以变量提升
2. `let` 定义的变量，<u>只能在块作用域里访问</u>（不能跨块访问，也不能跨函数访问）<u>无变量提升，不可以重复声明</u>
3. `const` 用来定义常量，使用时必须初始化 (即必须赋值)，且不能修改，<u>只能在块作用域里访问，无变量提升，不可以重复声明</u>

```js
let
//Only needed when create a variable for the first time
const
//By default
//Unable to change/re-assign the value
var
//Old
```

#### 1. `let` 和 `const` 声明的变量只在块级作用域内有效，示例

```js
function func() {
  if (true) {
    let i = 3;
  }
  console.log(i); // 报错 "i is not defined"
}
func();
```

#### 2. `var` 与 `let` 的经典案例
1） 用 var 定义 i 变量，循环后打印 i 的值

```js
// 案例1
// i是var声明的，在全局范围内都有效，全局只有一个变量i，输出的是最后一轮的i值，也就是 10

var a = [];
for (var i = 0; i < 10; i++) {
  a[i] = function() {
    console.log(i);
  };
}
a[0]();  // 10

```

2） 用 let 定义 i 变量，循环后打印 i 的值

```js
// 案例2
// 用let声明i，for循环体内部是一个单独的块级作用域，相互独立，不会相互覆盖
var a = [];
for (let i = 0; i < 10; i++) {
  a[i] = function() {
    console.log(i);
  };
}
a[0](); // 0
```

#### 3. let 实现原理
借助 **闭包**[[Closures-闭包]] 和函数作用域 [[Scope-作用域]] 来实现块级作用域的效果

```js
// 用var实现案例2的效果
var a = [];
var _loop = function _loop(i) {
  a[i] = function() {
    console.log(i);
  };
};
for (var i = 0; i < 10; i++) {
  _loop(i);
}
a[0](); // 0
```