---
title: Prototype Inheritance
tags: JS  
started: 2022-12-02 Fri
due: 
modified: 2022-12-05 Mon
status: 
---
>[Inheritance and the prototype chain - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain)  
>[Object prototypes - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object_prototypes)

## What is Prototype
Prototype: 
- mechanism by which JavaScript Objects **inherit** features from one another
- a powerful and very flexible feature of JavaScript, making it possible to reuse code and combine objects.
- Every Object in JavaScript has a built-in property called **prototype**, which is itself an [[Object]].  
Prototype Chain: 
- The prototype will have its own prototype, making what's called a **prototype chain**. 
- The chain ends when we reach a prototype that has `null` for its own prototype.
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

#### 2. Use Constructors
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