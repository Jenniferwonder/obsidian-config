---
Title: O-Object
tags: JavaScript
Type: Scope
DateStarted: 2022-12-01
DateModified: 2023-07-13
status:
aliases: Object
mindmap-plugin: basic
---

# O-[[O-JS|JS]] Object

## Metadata
- Reference
    - [Working with objects - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects)
    - [Introducing JavaScript objects - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects)
- Relationship
    - Related:: [[O-JS Data Types]]

## What is Object in JS?
- A collection of **Key-Value** Pairs, composed of
    - Key/ Property (属性)
    - Value
- A Reference Type
- There are many Built-in Objects in JS
- <mark class="hltr-yellow ">  </mark> Each Object instance has the following properties (属性) and methods (方法): [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=WKCAQ46A)
    - <mark class="hltr-orange ">  </mark> constructor [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=H2K26ZTJ)
        - Every Object has a property called 'constructor', refering to the [[O-JS Object#3. ✅Constructor(构造器) Function|Constructor Function]] that is used to create that object
    - <mark class="hltr-orange ">  </mark> hasOwnProperty(propertyName) [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=JPTDGMQ3)
    - <mark class="hltr-orange ">  </mark> isPrototypeof(object) [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=P8LZY6NZ)
    - <mark class="hltr-orange ">  </mark> propertyIsEnumerable(propertyName) [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=U59R7JH8)
    - <mark class="hltr-orange ">  </mark> toLocaleString() [Page 44 ](zotero://open-pdf/library/items/2BS329KQ?page=44&annotation=2JNWRVMG)
    - <mark class="hltr-orange ">  </mark> toString() [Page 44 ](zotero://open-pdf/library/items/2BS329KQ?page=44&annotation=VYD53SXR)
    - <mark class="hltr-orange ">  </mark> valueOf() [Page 44 ](zotero://open-pdf/library/items/2BS329KQ?page=44&annotation=6M3V9IUB)
- Built-in Objects in JS
    - [Standard built-in objects - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)
    - [[O-JS Array]]
    - [[O-JS Object]]
    - [[O-JS Number]]
    - [[O-JS Math]]
    - [[O-JS Date]]
    - [[O-JS Function]]
    - [[JSON]]
    - [[Fetch API]] - Request, Response

## How to Create Object?
-
    - <mark class="hltr-yellow ">  </mark> Objects are created by using the new operator followed by the name of the object type to create [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=ZHCMRL4M)
        - <mark class="hltr-orange ">  </mark> let o = new Object (); [Page 43 ](zotero://open-pdf/library/items/2BS329KQ?page=43&annotation=6SAPDPVY)
    - 1. ⛔Object literal (对象字面量) syntax: `{ }`

-
  ```js
  let x = {}; // let x = new Object{};
  // Other built-in constructors and literals
  new String(); // '', "", ``
  new Boolean(); // true, false
  new Number(); // 1, 2, 3...
  new Function(`arg`, ``); // function(`arg`){}
  new Error();
  ```


-
  ```js
  // Object literal syntax
  const circle = {
          radius: 1,
          location: {
                  x: 1,
                  y: 1,
          },
          draw: function () {
                  console.log("draw");
          },
  };
  circle.draw();
  ```

-
    - 2. ⛔Factory Function

-
  ```js
  // Factory Function
  function createCircle(radius) {
          return {
                  radius,
                  draw: function () {
                          console.log("draw");
                  },
          };
  }
  const circle = createCircle(1);
  ```

-
    - 3. ✅Constructor(构造器) Function

-
  ```js
  // Constructor Function
  function Circle(radius) {
          this.radius = radius;
          this.draw = function () {
                  console.log("draw");
          };
  }
  const another = new Circle(1);
  ```

-
    - 4. Destructuring 🟨

-
  ```js
  const {key:`varName`} = variable
  //store the property value of an object into a variable based on the property key
  ```


## Properties
-
    - Add/ Remove Property
        - dot notation (点表示法) `obj.propname = ...`
        - bracket notation: `obj['propname'] = ...`
        - can be used when property name is **invalid** to be accessed by dot
        - can be used when property name is **dynamically** changing
    - Delete property
        - `delete obj.propname/ obj['propname']`
    - How to access value?
        - dot notation
        - bracket notation: `[' ']`
    - How to access key/property?

-
  ```js
  for (let key in circle) {
  console.log(key, circle[key]); // return key and value
  }
  const keys = Object.keys(obj); // return an array of keys`
  ```

-
    - Private Properties

-
  ```js
  function Circle(radius) {
  this.radius = radius;
  // Use 'let' to convert properties into variables only available inside this scope
  let defaultLocation = { x: 0, y: 0 };
  let computeLocation = function (factor) {};
  // Closure enables the parent function variable is accessble to its child without 'this' keyword
  this.draw = function () {
      computeLoaction(0.1);
      console.log("draw");
  };
  }
  const circle = new Circle(10);
  circle.draw();
  ```

-
    - Getters/ Setters

-
  ```js
  {
          Object.defineProperty(this, "defaultlocation", {
                  get: function () {
                          return defaultLocation;
                  },
                  set: function (value) {
                          if (!value.x || !value.y) throw new Error("Invalid Location");
                          defaultLocation = value;
                  },
          });
  }
  const circle = new Circle(10);
  circle.defaultLocation = 1; // Return error message
  ```

-
    - CASE - Stop Watch-Reference: [[O-JS Date|O-JS Date]]

-
  ```js
  // Stopwatch Constructor Function
  function Stopwatch(){
          let startTime, endTime, running, duration = 0;
          this.start = function {
                  if (running)
                          throw new Error('Stopwatch has already started.')
                  running = true;
                  startTime = new Date
          };
          this.stop = function {
                  if(!running)
                          throw new Error('stopwatch is not started.');
                  running = false;
                  endTime = new Date();
                  const seconds = ((endTime.getTime() - startTime.getTime()) / 1000;
                  duration += seconds;
          };
          this.reset = function {
                  startTime = null;
                  endTime = null;
                  running = false;
                  duration = 0;
          };
          Object.defineProperty(this, 'duration', {
                  get: function(){ return duration; }
          });
  }
  // Use Stopwatch
  const sw = new Stopwatch()
  sw.start
  ```


## Methods
-
    - ES6 enhanced object literals 🟨
        - Create [[O-JS Function]] as **methods** inside an object
    - Object Built-in Methods

-
  ```js
  this.Object.assign(
          //Refer to the object calling the function (except arrow function in which 'this' refers to its parent object)
          {},
          `objectName`
  );
  //create a new object by merging existing objects together
  Object.freeze({});
  //make property in the object immutable. i.e. unable to add new properties, but the value inside a deeper level is mutable
  //work better in strict mode
  ```


## [[JS-OOP and Inheritance]]