---
title: this,call,apply,bind
tags: JS
started: 2022-12-16 Fri
due:
modified: 2022-12-16 Fri
status:
---
## Questions
- [面试官为啥总是让我们手撕call、apply、bind? - 掘金](https://juejin.cn/post/7128233572380442660)  
- [JavaScript基础心法——this](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Faxuebin%2Farticles%2Fissues%2F6 "https://github.com/axuebin/articles/issues/6")
-   [JavaScript深入之从ECMAScript规范解读this](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fmqyqingfeng%2FBlog%2Fissues%2F7 "https://github.com/mqyqingfeng/Blog/issues/7")
-   [前端基础进阶（七）：全方位解读this](https://link.juejin.cn?target=https%3A%2F%2Fwww.jianshu.com%2Fp%2Fd647aa6d1ae6 "https://www.jianshu.com/p/d647aa6d1ae6")
-   [面试官问：JS的this指向](https://juejin.cn/post/6844903746984476686 "https://juejin.cn/post/6844903746984476686")
-   [JavaScript深入之call和apply的模拟实现](https://juejin.cn/post/6844903476477034510 "https://juejin.cn/post/6844903476477034510")
-   [JavaScript基础心法—— call apply bind](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Faxuebin%2Farticles%2Fissues%2F7 "https://github.com/axuebin/articles/issues/7")
-   [面试官问：能否模拟实现JS的call和apply方法](https://juejin.cn/post/6844903728147857415 "https://juejin.cn/post/6844903728147857415")
-   [回味JS基础:call apply 与 bind](https://juejin.cn/post/6844903444348665870 "https://juejin.cn/post/6844903444348665870")
-   [面试官问：能否模拟实现JS的bind方法](https://juejin.cn/post/6844903718089916429 "https://juejin.cn/post/6844903718089916429")
-   [不用call和apply方法模拟实现ES5的bind方法](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fjawil%2Fblog%2Fissues%2F16 "https://github.com/jawil/blog/issues/16")
## `this`
>[再来40道this面试题酸爽继续(1.2w字用手整理)](https://juejin.cn/post/6844904083707396109 "https://juejin.cn/post/6844904083707396109")
#### 1. this的5种绑定方式
1）默认绑定(非严格模式下this指向全局对象，严格模式下函数内的this指向`undefined`)
2）隐式绑定(当函数引用有上下文对象时, 如 `obj.foo()`的调用方式, foo内的this指向obj)
3）显示绑定(通过call或者apply方法直接指定this的绑定对象, 如`foo.call(obj)`)
4）new构造函数绑定，this指向新生成的对象
5）箭头函数，this指向的是定义该函数时，外层环境中的this，**箭头函数的this在定义时就决定了，不能改变**
#### 2. this 题目1

```javascript
"use strict";
var a = 10; // var定义的a变量挂载到window对象上
function foo () {
  console.log('this1', this)  // undefined
  console.log(window.a)  // 10
  console.log(this.a)  //  报错，Uncaught TypeError: Cannot read properties of undefined (reading 'a')
}
console.log('this2', this)  // window
foo();
```

注意：开启了严格模式，只是使得函数内的this指向`undefined`，它并不会改变全局中this的指向。因此`this1`中打印的是`undefined`，而`this2`还是`window`对象。

#### 3. this 题目2

```javascript
let a = 10
const b = 20
function foo () {
  console.log(this.a)  // undefined
  console.log(this.b)  // undefined
}
foo();
console.log(window.a) // undefined  
复制代码
```

如果把 var 改成了 let 或 const，变量是不会被绑定到window上的，所以此时会打印出三个undefined

#### 4. this 题目3

```javascript
var a = 1
function foo () {
  var a = 2
  console.log(this)  // window
  console.log(this.a) // 1
}
foo()
```

foo()函数内的this指向的是window，因为是window调用的foo，打印出的`this.a`是window下的`a`

#### 5. this 题目4

```javascript
var obj2 = {
    a: 2,
    foo1: function () {
      console.log(this.a) // 2
    },
    foo2: function () {
      setTimeout(function () {
        console.log(this) // window
        console.log(this.a) // 3
      }, 0)
    }
  }
  var a = 3
  
  obj2.foo1()
  obj2.foo2() 
```

对于`setTimeout`中的函数，这里存在隐式绑定的this丢失，也就是当我们将函数作为参数传递时,会被隐式赋值，回调函数丢失this绑定，因此这时候setTimeout中函数内的this是指向`window`

#### 6. this 题目5

```javascript
var obj = {
 name: 'obj',
 foo1: () => {
   console.log(this.name) // window
 },
 foo2: function () {
   console.log(this.name) // obj
   return () => {
     console.log(this.name) // obj
   }
 }
}
var name = 'window'
obj.foo1()
obj.foo2()()
```

这道题非常经典，它证明了**箭头函数内的this是由外层作用域决定的**
##### 6.1. 题目5解析：  
1）对于`obj.foo1()`函数的调用，它的外层作用域是window，对象obj当然不属于作用域了(作用域只有全局作用域、函数作用域、块级作用域)，所以会打印出`window`
2）`obj.foo2()()`，首先会执行`obj.foo2()`，这不是个箭头函数，所以它里面的this是调用它的obj对象，因此第二个打印为`obj`，而返回的匿名函数是一个箭头函数，**它的this由外层作用域决定**，那也就是它的this会和foo2函数里的this一样，第三个打印也是`obj`
## call apply bind
#### 1. 三者的区别
1）三者都可以显式绑定函数的this指向
2）三者第一个参数都是this要指向的对象，若该参数为undefined或null，this则默认指向全局window
3）传参不同：apply是数组、call是参数列表，而bind可以分为多次传入，实现参数的合并
4）call、apply是立即执行，bind是返回绑定this之后的函数，如果这个新的函数作为构造函数被调用，那么this不再指向传入给bind的第一个参数，而是指向新生成的对象
#### 2. 手写call apply bind
```js
// 手写call
Function.prototype.Call = function(context, ...args) {
  // context为undefined或null时，则this默认指向全局window
  if (!context || context === null) {
    context = window;
  }
  // 利用Symbol创建一个唯一的key值，防止新增加的属性与obj中的属性名重复
  let fn = Symbol();
  // this指向调用call的函数
  context[fn] = this; 
  // 隐式绑定this，如执行obj.foo(), foo内的this指向obj
  let res = context[fn](...args);
  // 执行完以后，删除新增加的属性
  delete context[fn]; 
  return res;
};

// apply与call相似，只有第二个参数是一个数组，
Function.prototype.Apply = function(context, args) {
  if (!context || context === null) {
    context = window;
  }
  let fn = Symbol();
  context[fn] = this;
  let res = context[fn](...args);
  delete context[fn];
  return res;
};

// bind要考虑返回的函数，作为构造函数被调用的情况
Function.prototype.Bind = function(context, ...args) {
  if (!context || context === null) {
    context = window;
  }
  let fn = this;
  let f = Symbol();
  const result = function(...args1) {
    if (this instanceof fn) {
      // result如果作为构造函数被调用，this指向的是new出来的对象
      // this instanceof fn，判断new出来的对象是否为fn的实例
      this[f] = fn;
      let res = this[f](...args, ...args1);
      delete this[f];
      return res;
    } else {
      // bind返回的函数作为普通函数被调用时
      context[f] = fn;
      let res = context[f](...args, ...args1);
      delete context[f];
      return res;
    }
  };
  // 如果绑定的是构造函数 那么需要继承构造函数原型属性和方法
  // 实现继承的方式: 使用Object.create
  result.prototype = Object.create(fn.prototype);
  return result;
};
```
