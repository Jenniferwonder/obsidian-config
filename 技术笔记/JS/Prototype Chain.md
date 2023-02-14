---
title: Prototype Chain
tags: Front-End/JS  
started: 2022-12-02 Fri
due: 
modified: 2022-12-05 Mon
status: 
---
>[Inheritance and the prototype chain - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)  
>[Object prototypes - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object_prototypes)

## Questions
- [一文吃透所有JS原型相关知识点](https://juejin.cn/post/6844903984335945736 "https://juejin.cn/post/6844903984335945736")  
- [最详尽的 JS 原型与原型链终极详解](https://link.juejin.cn?target=https%3A%2F%2Fwww.jianshu.com%2Fp%2Fdee9f8b14771 "https://www.jianshu.com/p/dee9f8b14771")
-   [深入理解 JavaScript 原型](https://link.juejin.cn?target=https%3A%2F%2Fmp.weixin.qq.com%2Fs%2F1UDILezroK5wrcK-Z5bHOg "https://mp.weixin.qq.com/s/1UDILezroK5wrcK-Z5bHOg")
-   [【THE LAST TIME】一文吃透所有JS原型相关知识点](https://juejin.cn/post/6844903984335945736 "https://juejin.cn/post/6844903984335945736")
-   [重新认识构造函数、原型和原型链](https://juejin.cn/post/6844903779079290887 "https://juejin.cn/post/6844903779079290887")
-   [JavaScript深入之从原型到原型链](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fmqyqingfeng%2Fblog%2Fissues%2F2 "https://github.com/mqyqingfeng/blog/issues/2")
-   [最详尽的 JS 原型与原型链终极详解，没有「可能是」。（一）](https://link.juejin.cn?target=https%3A%2F%2Fwww.jianshu.com%2Fp%2Fdee9f8b14771 "https://www.jianshu.com/p/dee9f8b14771")
-   [最详尽的 JS 原型与原型链终极详解，没有「可能是」。（二）](https://link.juejin.cn?target=https%3A%2F%2Fwww.jianshu.com%2Fp%2F652991a67186 "https://www.jianshu.com/p/652991a67186")
-   [最详尽的 JS 原型与原型链终极详解，没有「可能是」。（三）](https://link.juejin.cn?target=https%3A%2F%2Fwww.jianshu.com%2Fp%2Fa4e1e7b6f4f8 "https://www.jianshu.com/p/a4e1e7b6f4f8")
-   [JavaScript 引擎基础：原型优化](https://link.juejin.cn?target=https%3A%2F%2Fhijiangtao.github.io%2F2018%2F08%2F21%2FPrototypes%2F "https://hijiangtao.github.io/2018/08/21/Prototypes/")
-   [Prototypes in JavaScript](https://link.juejin.cn?target=https%3A%2F%2Fmedium.com%2Fbetter-programming%2Fprototypes-in-javascript-5bba2990e04b "https://medium.com/better-programming/prototypes-in-javascript-5bba2990e04b")
-   [JavaScript深入之创建对象的多种方式以及优缺点](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fmqyqingfeng%2FBlog%2Fissues%2F15 "https://github.com/mqyqingfeng/Blog/issues/15")
-   [详解JS原型链与继承](https://link.juejin.cn?target=http%3A%2F%2Flouiszhai.github.io%2F2015%2F12%2F15%2FprototypeChain%2F "http://louiszhai.github.io/2015/12/15/prototypeChain/")
-   [从__proto__和prototype来深入理解JS对象和原型链](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fcreeperyang%2Fblog%2Fissues%2F9 "https://github.com/creeperyang/blog/issues/9")
-   [代码复用模式](https://link.juejin.cn?target=https%3A%2F%2Fgithub.com%2Fjayli%2Fjavascript-patterns%2Fblob%2Fmaster%2Fchapter6.markdown "https://github.com/jayli/javascript-patterns/blob/master/chapter6.markdown")
-   [JavaScript 中的继承：ES3、ES5 和 ES6](https://link.juejin.cn?target=http%3A%2F%2Ftianfangye.com%2F2017%2F12%2F31%2Finheritance-in-javascript-es3-es5-and-es6%2F "http://tianfangye.com/2017/12/31/inheritance-in-javascript-es3-es5-and-es6/")

## What is Prototype
#### 1. Prototype
- 原型被定义为给其它对象提供共享属性的对象，函数的实例可以共享原型上的属性和方法
- mechanism by which JavaScript Objects **inherit** features from one another
- a powerful and very flexible feature of JavaScript, making it possible to reuse code and combine objects.
- Every Object in JavaScript has a built-in property called **prototype**, which is itself an [[Object]].  
#### 2. Prototype Chain 
- The prototype will have its own prototype, making what's called a **prototype chain**. 
- The chain ends when we reach a prototype that has `null` for its own prototype.
- 它的作用就是当你在访问一个对象上属性的时候，如果该对象内部不存在这个属性，那么就会去它`__proto__`属性所指向的对象（原型对象）上查找。如果原型对象依旧不存在这个属性，那么就会去其原型的`__proto__`属性所指向的原型对象上去查找。以此类推，直到找到`nul`，而这个查找的线路，也就构成了我们常说的**原型链**
## How to access an object's prototype?
- [`Object.getPrototypeOf()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/getPrototypeOf)
- `objName.`  
Property shadowing: 
- when an object's property name is the same as the property name of its prototype
## How to set a Prototype?
#### 1. `Object.create()`
- creates a new object and allows you to specify an object that will be used as the new object's prototype

```js
const personPrototype = {
  greet() {
    console.log("hello!");
  },
};

const carl = Object.create(personPrototype);
carl.greet(); // hello!

```

#### 2. `Object.assign()` - Use Constructors
- It's common to see this pattern, in which **methods** are defined on the prototype, but data **properties** are defined in the constructor.

```js
const personPrototype = {
  greet() {
    console.log(`hello, my name is ${this.name}!`);
  },
};

function Person(name) {
  this.name = name;
}

Object.assign(Person.prototype, personPrototype);
// or
// Person.prototype.greet = personPrototype.greet;

```
## proto、prototype、constructor属性介绍
1）js中对象分为两种，普通对象和函数对象
2）`__proto__`和`constructor`是对象独有的。`prototype`属性是函数独有的，它的作用是包含可以给特定类型的所有实例提供共享的属性和方法；但是在 JS 中，函数也是对象，所以函数也拥有`__proto__`和 `constructor`属性
3）`constructor`属性是对象所独有的，它是一个对象指向一个函数，这个函数就是该对象的构造函数  
`构造函数.prototype.constructor === 该构造函数本身`
4）一个对象的`__proto__`指向其构造函数的`prototype`  
`函数创建的对象.__proto__ === 该函数.prototype`
5）特殊的`Object`、`Function`
```javascript
console.log(Function.prototype === Function.__proto__); // true
console.log(Object.__proto__ === Function.prototype); // true
console.log(Function.prototype.__proto__ === Object.prototype); // true
console.log(Object.prototype.__proto__ === null); // true
```

## instanceof
`instanceof` 的基本用法，它可以判断一个对象的原型链上是否包含该构造函数的原型，经常用来判断对象是否为该构造函数的实例
#### 1. 特殊示例
```javascript
console.log(Object instanceof Object); //true
console.log(Function instanceof Function); //true
console.log(Function instanceof Object); //true
console.log(function() {} instanceof Function); //true
```

#### 2. 手写instanceof方法

```javascript
function instanceOf(obj, fn) {
  let proto = obj.__proto__;
  if (proto) {
    if (proto === fn.prototype) {
      return true;
    } else {
      return instanceOf(proto, fn);
    }
  } else {
    return false;
  }
}
// 测试
function Dog() {}
let dog = new Dog();
console.log(instanceOf(dog, Dog), instanceOf(dog, Object)); // true true
```

#### 3. instanceof与typeof的区别
1）`typeof`一般被用于来判断一个变量的类型  
- typeof可以用来判断`number、undefined、symbol、string、function、boolean、object` 这七种数据类型，特殊情况：`typeof null === 'object'`
2）`instanceof`判断一个对象的原型链上是否包含该构造函数的原型

## new 关键字
#### 1. new一个对象，到底发生什么？
1）创建一个对象，该对象的原型指向构造函数的原型
2）调用该构造函数，构造函数的this指向新生成的对象
3）判断构造函数是否有返回值，如果有返回值且返回值是一个对象或一个方法，则返回该值；否则返回新生成的对象
#### 2. 构造函数有返回值的案例

```js
function Dog(name) {
  this.name = name;
  return { test: 1 };
}
let obj = new Dog("ming");
console.log(obj); // {test:1} 
```

#### 3. 手写new

```javascript
function selfNew(fn, ...args) {
  // 创建一个instance对象，该对象的原型是fn.prototype
  let instance = Object.create(fn.prototype);
  // 调用构造函数，使用apply，将this指向新生成的对象
  let res = fn.apply(instance, args);
  // 如果fn函数有返回值，并且返回值是一个对象或方法，则返回该对象，否则返回新生成的instance对象
  return typeof res === "object" || typeof res === "function" ? res : instance;
}
复制代码
```

## 继承——How to set a Prototype?
#### 1. 多种继承方式
1）原型链继承，缺点：引用类型的属性被所有实例共享  
2）借用构造函数（经典继承）  
3）原型式继承  
4）寄生式继承  
5）组合继承  
6）寄生组合式继承
#### 2. 寄生组合式继承
优势：借用父类的构造函数，在不需要生成父类实例的情况下，继承了父类原型上的属性和方法

```javascript
// 精简版
class Child {
  constructor() {
    // 调用父类的构造函数
    Parent.call(this);
    // 利用Object.create生成一个对象，新生成对象的原型是父类的原型，并将该对象作为子类构造函数的原型，继承了父类原型上的属性和方法
    Child.prototype = Object.create(Parent.prototype);
    // 原型对象的constructor指向子类的构造函数
    Child.prototype.constructor = Child;
  }
}

// 通用版
function Parent(name) {
  this.name = name;
}
Parent.prototype.getName = function() {
  console.log(this.name);
};
function Child(name, age) {
  // 调用父类的构造函数
  Parent.call(this, name); 
  this.age = age;
}
function createObj(o) {
  // 目的是为了继承父类原型上的属性和方法，在不需要实例化父类构造函数的情况下，避免生成父类的实例，如new Parent()
  function F() {}
  F.prototype = o;
  // 创建一个空对象，该对象原型指向父类的原型对象
  return new F(); 
}

// 等同于 Child.prototype = Object.create(Parent.prototype)
Child.prototype = createObj(Parent.prototype); 
Child.prototype.constructor = Child;

let child = new Child("tom", 12);
child.getName(); // tom
```



  
