---
Title: Scope
tags: JS
DateStarted: 2022-11-30
due:
DateModified: 2022-12-01
status:
---

## Questions

- [JavaScript 深入之作用域链](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fmqyqingfeng%2FBlog%2Fissues%2F6 "https://github.com/mqyqingfeng/Blog/issues/6")
- [js 块级作用域和 let，const，var 区别](https://link.juejin.cn?target=https%3A%2F%2Fwww.cnblogs.com%2Fmoumoon%2Fp%2F10985250.html "https://www.cnblogs.com/moumoon/p/10985250.html")
- [JavaScript 深入之词法作用域和动态作用域](https://link.juejin.cn/?target=https%3A%2F%2Fgithub.com%2Fmqyqingfeng%2FBlog%2Fissues%2F3 "https://github.com/mqyqingfeng/Blog/issues/3")

## Scope

! Refers to the environment where a certain variable is declared;  
! JS => Lexical scoping which is defined by the placement of functions and blocks in the code  
! Scope of a variable: Refer to the entire region of code where a certain variable can be accessed  
作用域：可访问变量的集合
作用域最大的用处就是`隔离变量`，不同作用域下同名变量不会有冲突

## Three Types of Scope 作用域类型

#### 1. Global scope 全局作用域

#### 2. Function scope/ Local scope 函数作用域

是指声明在函数内部的变量，函数的作用域在函数定义的时候就决定了

#### 3. Block scope ES6 块级作用域

> [[Value and Variables]]

- 块作用域由`{ }`包括，if 和 for 语句里面的`{ }`也属于块作用域
  - Eg. if/ for loops
- 在块级作用域中，可通过 let 和 const 声明变量，该变量在指定块的作用域外无法被访问
  - let; const (not var)

## 作用域链

当查找变量的时候，首先会先从当前上下文的变量对象（作用域）中查找，如果没有找到，就会从父级的执行上下文的变量对象中查找，如果还没有找到，一直找到全局上下文的变量对象，也就是全局对象。这样由多个执行上下文的变量对象构成的链表就叫做`作用域链`
! Child scope can access variables in its parent scope
