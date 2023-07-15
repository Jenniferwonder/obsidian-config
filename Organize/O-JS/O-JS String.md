---
Title: O-String
tags: JavaScript
Type: Scope
DateStarted: 2022-12-01
DateModified: 2023-07-13
status:
aliases: String
mindmap-plugin: basic
---

# [[O-JS]] String

## Metadata
- Reference:: [Useful string methods - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Useful_string_methods)
- Related:: [[O-JS C03-Language Basics]]

## <mark class="hltr-gray ">" Character Literals "</mark> [Page 23 ]( zotero://open-pdf/library/items/2BS329KQ?page=23&annotation=8XCJSYWK )
- <mark class="hltr-yellow ">" to represent nonprintable or otherwise useful characters "</mark> [Page 23 ]( zotero://open-pdf/library/items/2BS329KQ?page=23&annotation=B86AUNZD )
- Multiple lines
    - `\n\`
    - `hit enter
- ![[zz-assets/Zotero/C3LanguageBasics/C3LanguageBasics-23-x75-y192.png]]
- <mark class="hltr-orange ">" The length of any string "</mark> [Page 23 ]( zotero://open-pdf/library/items/2BS329KQ?page=23&annotation=GFPCVAED)
    - <mark class="hltr-yellow ">" console.log(text.length); "</mark> [Page 23 ]( zotero://open-pdf/library/items/2BS329KQ?page=23&annotation=34YKN38S)

## <mark class="hltr-gray ">" The Nature of Strings "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=65YKGC7R )
- <mark class="hltr-yellow ">" Strings are immutable in ECMAScript "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=X8XTAY2R )
- <mark class="hltr-yellow ">" To change the string held by a variable, the original string must be destroyed and the variable filled with another string containing a new value "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=RP7Q3XY6 )

## <mark class="hltr-gray ">" Converting to a String "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=2VIU36Z9 )
- <mark class="hltr-orange ">" use the toString() method"</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=G49YDI7P )
    - <mark class="hltr-yellow ">" If a value is null or undefined, this method is not available. "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=ZF6GC5ZZ)
    - <mark class="hltr-yellow ">" when used on a number value, toString() actually accepts a single argument: the radix "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=9CDMY2I9)
    - <mark class="hltr-yellow ">" output the value in binary, octal, hexadecimal, or any other valid base "</mark> [Page 24 ]( zotero://open-pdf/library/items/2BS329KQ?page=24&annotation=X9BN2PR9)
- <mark class="hltr-orange ">" String() casting function "</mark> [Page 25 ]( zotero://open-pdf/library/items/2BS329KQ?page=25&annotation=5YMDD2NP)
    - <mark class="hltr-yellow ">" always returns a string regardless of the value type. "</mark> [Page 25 ]( zotero://open-pdf/library/items/2BS329KQ?page=25&annotation=TGJ8UD3U)

## <mark class="hltr-gray ">" Template Literals "</mark> [Page 25 ]( zotero://open-pdf/library/items/2BS329KQ?page=25&annotation=9XL2ANQR )
- Template literals (模板字面量/字符串) `I'm ${firstName}`
- <mark class="hltr-yellow ">" template literals respect new line characters, and can be defined spanning multiple lines "</mark> [Page 25 ]( zotero://open-pdf/library/items/2BS329KQ?page=25&annotation=YD5JG86Y )
- <mark class="hltr-yellow ">" template literals are especially useful when defining templates, such as HTML "</mark> [Page 26 ]( zotero://open-pdf/library/items/2BS329KQ?page=26&annotation=9YBXMQAG)
- <mark class="hltr-yellow ">" template literals will exactly match the whitespace inside the backticks "</mark> [Page 26 ]( zotero://open-pdf/library/items/2BS329KQ?page=26&annotation=C7IR9YKH)
- <mark class="hltr-yellow ">" A correctly formatted template string may appear to have improper indentation "</mark> [Page 26 ]( zotero://open-pdf/library/items/2BS329KQ?page=26&annotation=FEJZ3JSB)
- <mark class="hltr-gray ">" Interpolation "</mark> [Page 26 ]( zotero://open-pdf/library/items/2BS329KQ?page=26&annotation=4MWTRXQB )
    - <mark class="hltr-yellow ">" allows you to insert values at one or more places inside a single unbroken definition. "</mark> [Page 26 ]( zotero://open-pdf/library/items/2BS329KQ?page=26&annotation=XNZ67VF2 )
    - <mark class="hltr-yellow ">" Invoking functions and methods inside interpolated expressions is allowed "</mark> [Page 27 ]( zotero://open-pdf/library/items/2BS329KQ?page=27&annotation=SQV53TFZ )
- <mark class="hltr-gray ">" Template Literal Tag Functions "</mark> [Page 27 ]( zotero://open-pdf/library/items/2BS329KQ?page=27&annotation=G5Q823M9 )
    - <mark class="hltr-orange ">" tag functions "</mark> [Page 27 ]( zotero://open-pdf/library/items/2BS329KQ?page=27&annotation=5ZDI7IBD )
    - <mark class="hltr-yellow ">" are able to define custom interpolation behavior. "</mark> [Page 27 ]( zotero://open-pdf/library/items/2BS329KQ?page=27&annotation=93HCMA8N )
    - <mark class="hltr-yellow ">" A tag function is defined as a regular function and is applied to a template literal by being prepended to it, "</mark> [Page 27 ]( zotero://open-pdf/library/items/2BS329KQ?page=27&annotation=9YYK4IQN )

## <mark class="hltr-gray ">" Raw Strings "</mark> [Page 29 ]( zotero://open-pdf/library/items/2BS329KQ?page=29&annotation=E2RSKQVV)
- <mark class="hltr-orange ">" String. raw tag function "</mark> [Page 29 ]( zotero://open-pdf/library/items/2BS329KQ?page=29&annotation=ACA4B23P )
- <mark class="hltr-yellow ">" console. log (String.raw`first line\nsecond line`); // "first line\nsecond line" "</mark> [Page 29 ]( zotero://open-pdf/library/items/2BS329KQ?page=29&annotation=Q4JV4UI7 )

## String Concatenation
- How to join strings?
- Use [[O-JS Operators]] : `+=`

  ```js
  if (guessCount === 1) {
      guesses.textContent = `Previous guesses: `;
  }
  guesses.textContent += ` ${guess}`;
  ```


## String Methods
- Replace

```js
.replace(`original`, `new`)
.replace(/`original`/g, `new`)
//to replace all the same content
```

- Check if elements in a string
```js
.includes( )
.startsWith( )
.endsWith( )
```

- Split, Join and Add symbols

```js
.split('divider')
//to split the string by a divider in the string
.join(' ')
//to join split strings with a specified divider to one string
.padStart(20, '+')
.padEnd
//to add symbols to a string to a certain length
```

- Repeat a String

```js
.repeat(5)
//to repeat the string 5 times
```

- Convert Number to String

## <mark class="hltr-gray ">" The JavaScript Character "</mark> [Page 20 ]( zotero://open-pdf/library/items/6CRSJHBD?page=20&annotation=JMV7BFPH)

## <mark class="hltr-gray ">" The normalize() Method "</mark> [Page 23 ]( zotero://open-pdf/library/items/6CRSJHBD?page=23&annotation=6W4PEF9Y)

## <mark class="hltr-gray ">" String-Manipulation Methods "</mark> [Page 24 ]( zotero://open-pdf/library/items/6CRSJHBD?page=24&annotation=87P4LDHG)

## <mark class="hltr-gray ">" String Location Methods "</mark> [Page 26 ]( zotero://open-pdf/library/items/6CRSJHBD?page=26&annotation=K3CKKLCB)

## <mark class="hltr-gray ">" String Inclusion Methods "</mark> [Page 27 ]( zotero://open-pdf/library/items/6CRSJHBD?page=27&annotation=B9WYFDGA)

## <mark class="hltr-gray ">" The trim() Method "</mark> [Page 27 ]( zotero://open-pdf/library/items/6CRSJHBD?page=27&annotation=UHGAI8KR)

- Remove white space or new line in a string
  ```js
  .trim()
  ```


## <mark class="hltr-gray ">" The repeat() Method "</mark> [Page 28 ]( zotero://open-pdf/library/items/6CRSJHBD?page=28&annotation=HPTIT6M4)

## <mark class="hltr-gray ">" The padStart() and padEnd() Methods "</mark> [Page 28 ]( zotero://open-pdf/library/items/6CRSJHBD?page=28&annotation=4S9JYAE6)

## <mark class="hltr-gray ">" String Iterators and Destructuring "</mark> [Page 28 ]( zotero://open-pdf/library/items/6CRSJHBD?page=28&annotation=LZID94FV)

## <mark class="hltr-gray ">" String Case Methods "</mark> [Page 29 ]( zotero://open-pdf/library/items/6CRSJHBD?page=29&annotation=QJNZ78U8)

  ```js
  .toLowerCase()
  .toUpperCase()
  ```


## <mark class="hltr-gray ">" String Pattern-Matching Methods "</mark> [Page 29 ]( zotero://open-pdf/library/items/6CRSJHBD?page=29&annotation=Y9G2P237)

## <mark class="hltr-gray ">" The localeCompare() Method "</mark> [Page 32 ]( zotero://open-pdf/library/items/6CRSJHBD?page=32&annotation=EYLW8PV5)

## <mark class="hltr-gray ">" HTML Methods "</mark> [Page 33 ]( zotero://open-pdf/library/items/6CRSJHBD?page=33&annotation=F97NKWWU)