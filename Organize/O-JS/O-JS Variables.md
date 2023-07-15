---
Title: O-Value and Variable
tags: JavaScript
Type: Scope
DateStarted: 2022-12-02
DateModified: 2023-07-13
status:
mindmap-plugin: basic
---

# O-[[O-JS|JS]] Variables

## Metadata
- Reference:: [Storing the information you need — Variables - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Variables)

## Value and Variables
- 1. Value
    - [[O-JS Data Types#Primitive Data Type]]
- 2. Variable
    - A container that stores value
    - Dynamic Data Type

## `var`
- 定义的变量，没有块的概念，可以跨块访问, 可以变量提升
- <mark class="hltr-gray ">" var Declaration Scope "</mark> [Page 5 ]( zotero://open-pdf/library/items/2BS329KQ?page=5&annotation=9EMHNQLQ)
- <mark class="hltr-gray ">" var Declaration Hoisting "</mark> [Page 6 ]( zotero://open-pdf/library/items/2BS329KQ?page=6&annotation=5KRSMUUN)

-
  ```js
  // 案例1
  // i是var声明的，在全局范围内都有效，全局只有一个变量i，输出的是最后一轮的i值，也就是 10
  
  var a = [];
  for (var i = 0; i < 10; i++) {
      a[i] = function () {
          console.log(i);
      };
  }
  a[0](); // 10
  ```

- 借助 **闭包**[[Closures-闭包]] 和函数作用域 [[O-JS Scope-作用域]] 来实现块级作用域的效果

-
  ```js
  // 用var实现案例2的效果
  var a = [];
  var _loop = function _loop(i) {
      a[i] = function () {
          console.log(i);
      };
  };
  for (var i = 0; i < 10; i++) {
      _loop(i);
  }
  a[0](); // 0
  ```


## `let`
- 定义的变量，只能在块作用域 [[O-JS Scope-作用域]] 里访问（不能跨块访问，也不能跨函数访问）无变量提升，不可以重复声明
- <mark class="hltr-gray ">" Temporal Dead Zone "</mark> [Page 8 ]( zotero://open-pdf/library/items/2BS329KQ?page=8&annotation=CU8ZHDQX )
    - <mark class="hltr-yellow ">" cannot be used in a way that assumes hoisting "</mark> [Page 8 ]( zotero://open-pdf/library/items/2BS329KQ?page=8&annotation=38TNQNG8)
- <mark class="hltr-gray ">" Global Declarations "</mark> [Page 8 ]( zotero://open-pdf/library/items/2BS329KQ?page=8&annotation=WEUZDU2E )
    - <mark class="hltr-yellow ">" variables will not attach to the window object as they do with var "</mark> [Page 8 ]( zotero://open-pdf/library/items/2BS329KQ?page=8&annotation=ZZY7P3LC)
- <mark class="hltr-gray ">" Conditional Declaration "</mark> [Page 8 ]( zotero://open-pdf/library/items/2BS329KQ?page=8&annotation=69C5L7MM )
    - <mark class="hltr-yellow ">" conditionally declare it only if it has not "</mark> [Page 8 ]( zotero://open-pdf/library/items/2BS329KQ?page=8&annotation=4IMUWUY9 )
- <mark class="hltr-gray ">" let Declaration in for Loops "</mark> [Page 10 ]( zotero://open-pdf/library/items/2BS329KQ?page=10&annotation=M8N2ZSD9)

-
  ```js
  function func() {
      if (true) {
          let i = 3;
      }
      console.log(i); // 报错 "i is not defined"
  }
  func();
  ```


-
  ```js
  // 案例2
  // 用let声明i，for循环体内部是一个单独的块级作用域，相互独立，不会相互覆盖
  var a = [];
  for (let i = 0; i < 10; i++) {
      a[i] = function () {
          console.log(i);
      };
  }
  a[0](); // 0
  ```


## `const`
- 用来定义常量，使用时必须初始化 (即必须赋值)，且不能修改，只能在块作用域里访问，无变量提升，不可以重复声明
- <mark class="hltr-yellow ">" it must be initialized with a value "</mark> [Page 10 ]( zotero://open-pdf/library/items/2BS329KQ?page=10&annotation=ZUXGB5XK )
- <mark class="hltr-yellow ">" that value cannot be redefined after declaration "</mark> [Page 10 ]( zotero://open-pdf/library/items/2BS329KQ?page=10&annotation=AAJV7NMT )
- <mark class="hltr-yellow ">" you cannot use const to declare for loop iterators "</mark> [Page 11 ]( zotero://open-pdf/library/items/2BS329KQ?page=11&annotation=6NIQJB6R )

## <mark class="hltr-gray ">" Declaration Styles and Best Practices "</mark> [Page 11 ]( zotero://open-pdf/library/items/2BS329KQ?page=11&annotation=77PIZC25)
- <mark class="hltr-gray ">" Don’t Use var "</mark> [Page 12 ]( zotero://open-pdf/library/items/2BS329KQ?page=12&annotation=HY4UAB6Y)
- <mark class="hltr-gray ">" Prefer const Over let "</mark> [Page 12 ]( zotero://open-pdf/library/items/2BS329KQ?page=12&annotation=W8GCVGJV)

-
  ```js
  let
  //Only needed when create a variable for the first time
  const
  //By default
  //Unable to change/re-assign the value
  var
  //Old
  ```