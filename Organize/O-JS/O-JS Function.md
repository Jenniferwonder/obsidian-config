---
Title: O-JS Function
tags: JavaScript
Type: Scope
DateStarted: 2022-12-01
DateModified: 2023-07-14
status:
mindmap-plugin: basic
---

# [[O-JS]] Function

## Metadata
- Reference:: [Functions - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)

## Overview
- ![[Pasted image 20230310112955.png]]

## Use
- <mark class="hltr-yellow ">" allow the encapsulation of statements that can be run anywhere and at any time "</mark> [Page 74 ]( zotero://open-pdf/library/items/2BS329KQ?page=74&annotation=35XF5CA2 )
- <mark class="hltr-yellow ">" This function can then be called by using the function name, followed by the function arguments enclosed in parentheses "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=T4HHA7U9)

## Return
- <mark class="hltr-yellow ">" Functions in ECMAScript need not specify whether they return a value. "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=43VGQWZ2)
- <mark class="hltr-yellow ">" Any function can return a value at any time by using the return statement followed by the value to return. "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=L2TQEL3A)
- <mark class="hltr-yellow ">" a function stops executing and exits immediately when it encounters the return statement "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=3RV747WU)
    - <mark class="hltr-yellow ">" any code that comes after a return statement will never be executed. "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=GFGSHUYD )
- <mark class="hltr-yellow ">" The return statement can also be used without specifying a return value "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=F7TSCCXE)
    - <mark class="hltr-yellow ">" in this way, the function stops executing immediately and returns undefined as its value. "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=E5EXGBCW )
    - <mark class="hltr-yellow ">" used in functions that don’t return a value to stop function execution early "</mark> [Page 75 ]( zotero://open-pdf/library/items/2BS329KQ?page=75&annotation=BMMDLGYZ )
- <mark class="hltr-yellow ">" a function either always return a value or never return a value. "</mark> [Page 76 ]( zotero://open-pdf/library/items/2BS329KQ?page=76&annotation=NGCUJXR2)
- <mark class="hltr-orange ">" Strict mode "</mark> [Page 76 ]( zotero://open-pdf/library/items/2BS329KQ?page=76&annotation=J3IZR5J8)
    - <mark class="hltr-yellow ">" No function can be named eval or arguments. "</mark> [Page 76 ]( zotero://open-pdf/library/items/2BS329KQ?page=76&annotation=3AI3VGDZ )
    - <mark class="hltr-yellow ">" No named parameter can be named eval or arguments. "</mark> [Page 76 ]( zotero://open-pdf/library/items/2BS329KQ?page=76&annotation=944KSISL )
    - <mark class="hltr-yellow ">" No two named parameters can have the same name. "</mark> [Page 76 ]( zotero://open-pdf/library/items/2BS329KQ?page=76&annotation=V24DIKZ3 )

## Basics
-
    -
        - 1. Promp and Alert
    -

        -
          ```js
          promp("");
          //get user input
          alert();
          ```

-
    - 2. Default parameters
-
    -
        - 3. IIFE
    -
        -
            - immediately invoked function expression

        -

          ```JS
          (function( ) { } )( );
          ```

-
    -
        - 4. Closures
    -
        - to give a function access to all variables of its parent function, even after that parent function has returned

## Create a function
-
    -
        - 1. Function declaration 函数声明
    -
        -
            - Able to call the function before declaring it

        -

          ```js
          funtion funName (parameter> argument) { }
          ```

-
    -
        - 2. Function expression 函数表达式
    -
        -
            - An expression produces a value

        -

          ```js
          const funName = funtion (parameter> argument) { }
          ```

-
    -
        - 3. Arrow function (ES6)
    -
        - An expression produces a value
        - does not have its own "this" key word
        - "this" in arrow function refers to its parent object/ function
        - can not be constructor function in OOP

## Function Methods 🟨
-
    -
        - 1. Name
    -

        -
          ```js
          funName.name;
          //to get the name of the function
          ```

-
    -
        - 2. Call
    -

        -
          ```js
          funName.call(`newObjectName`, `function parameter`);
          //to apply the function with "this" inside an object to a new object
          ```

-
    - 3. Apply
-
    -
        - 4. Bind
    -

        -
          ```JS
          const newFunName = funName.bind(`newObjectName/ argument to event handlers`)
          //create a new function to apply the function with "this" inside an object to a new object
          const newFunName = funName.bind(`newObjectName`, `pre-set parameter`)
          ```