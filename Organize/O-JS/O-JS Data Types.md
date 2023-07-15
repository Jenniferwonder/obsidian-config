---
Title: O-JS Data Types
Type: Scope
tags: JavaScript
DateStarted: 2022-11-30
DateModified: 2023-07-14
status:
mindmap-plugin: basic
---

# [[O-JS]] Data Types

## Metadata
- Reference:: [JavaScript data types and data structures - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures)

## <mark class="hltr-gray ">" The typeof Operator "</mark> [Page 12 ]( zotero://open-pdf/library/items/2BS329KQ?page=12&annotation=6MWRG9EZ)
-
    - 1. Check value type

-
  ```js
  .typeof
  ```

- <mark class="hltr-yellow ">" typeof is an operator and not a function, no parentheses are required "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=XBIBFJ24 )
- <mark class="hltr-yellow ">" functions are considered objects in ECMAScript "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=IJBQDGX3)
- <mark class="hltr-yellow ">" they do have some special properties "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=KFFCYKFG)
- <mark class="hltr-yellow ">" differentiating between functions and other objects "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=C66UXU55)
- 7 Types

## <mark class="hltr-orange ">     </mark> six simple data types [Page 12 ](zotero://open-pdf/library/items/2BS329KQ?page=12&annotation=4IBPLLP4)
- <mark class="hltr-gray ">" The Undefined Type "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=H475ZUQH)
    - <mark class="hltr-yellow ">" The Undefined type has only one value, which is the special value undefined "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=6M4TKWE5 )
    - <mark class="hltr-yellow ">" explicitly initialized to be undefined. This is unnecessary "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=MDWPBW3M )
    - <mark class="hltr-yellow ">" to help formalize the difference between an empty object pointer (null) and an uninitialized variable "</mark> [Page 13 ]( zotero://open-pdf/library/items/2BS329KQ?page=13&annotation=I8QP28Z7 )
    - <mark class="hltr-yellow ">" The value undefined is falsy "</mark> [Page 14 ]( zotero://open-pdf/library/items/2BS329KQ?page=14&annotation=DC5NKRYH )
- <mark class="hltr-gray ">" The Null Type "</mark> [Page 15 ]( zotero://open-pdf/library/items/2BS329KQ?page=15&annotation=2UFKXM3M)
    - <mark class="hltr-yellow ">" Logically, a null value is an empty object pointer, which is why typeof returns "object" "</mark> [Page 15 ]( zotero://open-pdf/library/items/2BS329KQ?page=15&annotation=9LCN8WSG )
    - <mark class="hltr-yellow ">" Even though null and undefined are related, they have very different uses "</mark> [Page 15 ]( zotero://open-pdf/library/items/2BS329KQ?page=15&annotation=INMIDBYF )
    - <mark class="hltr-yellow ">" Any time an object is expected but is not available, null should be used in its place. "</mark> [Page 15 ]( zotero://open-pdf/library/items/2BS329KQ?page=15&annotation=Y9Z6NC8K )
    - <mark class="hltr-yellow ">" This helps to keep the paradigm of null as an empty object pointer and further differentiates it from undefined. "</mark> [Page 15 ]( zotero://open-pdf/library/items/2BS329KQ?page=15&annotation=QJGFJISV )
    - <mark class="hltr-yellow ">" The null type is falsy "</mark> [Page 15 ]( zotero://open-pdf/library/items/2BS329KQ?page=15&annotation=B3HF8R5F )
- The [[O-JS Boolean|Boolean]] Type
- The [[O-JS Number|Number]] Type
- The [[O-JS String|String]] Type
- The [[O-JS Symbol|Symbol]] Type (ES2015)
- Primitive Data Type 基本数据类型/原始数据类型
    - Copied by the value
    - Changing the copied value will not change the original variable value
- [[O-JS C04-Variables, Scope, Memory]]

## <mark class="hltr-orange ">     </mark> one complex data type [Page 12 ](zotero://open-pdf/library/items/2BS329KQ?page=12&annotation=TG6VRLM9)
- The [[O-JS Object|Object]] Type
- Reference Type 引用数据类型
    - Copied by their reference
    - will not independently copy the value, but only refer to the original
    - Changing the value will change the original
    - Other Built-in Objects
        - [[Projects/Front-End/Front-End Basics/JavaScript/JS Basics/Date|Date]]
        - [[O-JS Math]]
        - [[Error]] ❓(try...catch)
        - RegExp
    - Set (ES6)
    - Map (ES6)
    - [[Sets and Maps]]
- [[O-JS C05-Basic Reference Type]]
- [[O-JS C06-Collection Reference Type]]