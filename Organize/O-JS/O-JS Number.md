---
Title: O-Number
tags: JavaScript
Type: Scope
DateStarted: 2022-12-01 
DateModified: 2023-07-13
status:
mindmap-plugin: basic
---

# [[O-JS]] Number

## <mark class="hltr-yellow ">" uses the IEEE–754 format to represent both integers and floating-point values (also called double–precision values in some languages) "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=A5WZZFZV )

## Number Literal Formats
- <mark class="hltr-orange ">" Integers "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=FZRMQJER )
- <mark class="hltr-orange ">" octal literal "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=RQB6KWEC)
    - <mark class="hltr-yellow ">" the first digit must be a zero (0) followed by a sequence of octal digits (numbers 0 through 7). "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=YS29P5TB)
    - <mark class="hltr-yellow ">" Octal literals are invalid when running in strict mode "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=8Z3RHIEU)
- <mark class="hltr-orange ">" hexadecimal literal "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=XEY4B8AR)
    - <mark class="hltr-yellow ">" must make the first two characters 0x (case insensitive), followed by any number of hexadecimal digits (0 through 9, and A through F) "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=EX2ZTVDK)
    - <mark class="hltr-yellow ">" Numbers created using octal or hexadecimal format are treated as decimal numbers in all arithmetic operations. "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=JRHZCGE8)

## <mark class="hltr-gray ">" Floating-Point Values "</mark> [Page 17 ]( zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=T98XG2D7)
- <mark class="hltr-yellow ">  </mark> To define a floating-point value, you must include a decimal point and at least one number after the decimal point. [Page 17 ](zotero://open-pdf/library/items/2BS329KQ?page=17&annotation=RFDEY5S4)
- <mark class="hltr-yellow ">  </mark> ECMAScript always looks for ways to convert values into integers. [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=VJCLBKPX)
- <mark class="hltr-orange ">  </mark> e-notation [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=UN6QPP3C)
    - <mark class="hltr-yellow ">  </mark> used to indicate a number that should be multiplied by 10 raised to a given power [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=GRBMX4RG)
    - `let floatNum = 3.125e7; // equal to 31250000`
    - <mark class="hltr-yellow ">  </mark> Take 3.125 and multiply it by 10^7 [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=AJRNFWJC)
    - <mark class="hltr-yellow ">  </mark> 0.00000000000000003 [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=DDL55Z8D)
    - <mark class="hltr-yellow ">  </mark> 3e–17 [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=Y3MUJ2UR)
    - <mark class="hltr-yellow ">  </mark> ECMAScript converts any floating-point value with at least six zeros after the decimal point into e-notation [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=5BIM5XWJ)
- <mark class="hltr-orange ">  </mark> small rounding errors [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=BVKJB4XY)

## <mark class="hltr-gray ">" Range of Values "</mark> [Page 18 ]( zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=WHDRDPSG)
- <mark class="hltr-orange ">  </mark> Number.MIN_VALUE [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=2Q7TE89T)
    - <mark class="hltr-yellow ">  </mark> 5 e–324 [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=TBWBHHBJ)
- <mark class="hltr-orange ">  </mark> MAX_VALUE [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=QCNLPCQZ)
    - <mark class="hltr-yellow ">  </mark> 1.7976931348623157 e+308 [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=XX4PRL6W)
- <mark class="hltr-orange ">  </mark> –Infinity (negative infinity) [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=7WDWI9TZ)
    - <mark class="hltr-yellow ">  </mark> Any negative number that can’t be represented [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=GPX73K37)
- <mark class="hltr-orange ">  </mark> Infinity (positive infinity) [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=L4FL2HMR)
    - Infinity: 23 / 0
    - <mark class="hltr-yellow ">  </mark> any positive number that can’t be represented [Page 18 ](zotero://open-pdf/library/items/2BS329KQ?page=18&annotation=BGJFJG5Q)
    - <mark class="hltr-yellow ">  </mark> If a calculation returns either positive or negative Infinity, that value cannot be used in any further calculations [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=Z7TDBQRP)
- <mark class="hltr-orange ">  </mark> isFinite() function [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=QEYIC3VT)
    - <mark class="hltr-yellow ">  </mark> To determine if a value is finite (that is, it occurs between the minimum and the maximum) [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=C2KJJ5E7)
- <mark class="hltr-orange ">  </mark> Number.NEGATIVE _ INFINITY [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=46LC8L9X)
- <mark class="hltr-orange ">  </mark> Number.POSITIVE _ INFINITY [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=DAP4Z8CF)
- BigInt(ES2020)
    - The biggest number: `2 ** 53 - 1`
    - Only 53 bits are used in JS to store the digits; the rest are used to store decimals
    - Numbers are represented as 64 bits

## <mark class="hltr-gray ">" NaN "</mark> [Page 19 ]( zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=24WP33WV)
- not a number
- <mark class="hltr-yellow ">  </mark> any operation involving NaN always returns NaN [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=5VZ83BB9)

- <mark class="hltr-yellow ">  </mark> NaN is not equal to any value, including NaN [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=U4CXQP3U)

- <mark class="hltr-orange ">  </mark> isNaN() function [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=SKYWJJEA)

- <mark class="hltr-yellow ">  </mark> to determine if the value is “not a number.” [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=QWYI8S8G)
- <mark class="hltr-yellow ">  </mark> Any value that cannot be converted into a number causes the function to return true. [Page 19 ](zotero://open-pdf/library/items/2BS329KQ?page=19&annotation=M8ZM96DF)

## <mark class="hltr-gray ">" Number Conversions "</mark> [Page 20 ]( zotero://open-pdf/library/items/2BS329KQ?page=20&annotation=5TYX6IXZ )
-
    - <mark class="hltr-orange ">" Number() function "</mark> [Page 20 ]( zotero://open-pdf/library/items/2BS329KQ?page=20&annotation=67KS4CPB )
        - <mark class="hltr-yellow ">  </mark> applied to Boolean [Page 20 ](zotero://open-pdf/library/items/2BS329KQ?page=20&annotation=UHUJP7JG)
        - <mark class="hltr-yellow ">  </mark> applied to null [Page 20 ](zotero://open-pdf/library/items/2BS329KQ?page=20&annotation=XSU3JDYI)
        - <mark class="hltr-yellow ">  </mark> applied to undefined [Page 20 ](zotero://open-pdf/library/items/2BS329KQ?page=20&annotation=HF6XBEHL)
        - <mark class="hltr-yellow ">  </mark> applied to strings [Page 20 ](zotero://open-pdf/library/items/2BS329KQ?page=20&annotation=EFDF3MLW)
        - <mark class="hltr-orange ">  </mark> unary plus operator [Page 21 ](zotero://open-pdf/library/items/2BS329KQ?page=21&annotation=FC7LIRQT)
            - <mark class="hltr-yellow ">  </mark> works the same as the Number () function. [Page 21 ](zotero://open-pdf/library/items/2BS329KQ?page=21&annotation=HWIFNUEM)
    - <mark class="hltr-orange ">" parseInt() "</mark> [Page 21 ]( zotero://open-pdf/library/items/2BS329KQ?page=21&annotation=I7R8K26N)
        - <mark class="hltr-yellow ">" If this first character isn’t a number, the minus sign, or the plus sign, parseInt() always returns NaN "</mark> [Page 21 ]( zotero://open-pdf/library/items/2BS329KQ?page=21&annotation=KRFNH8EF)
        - <mark class="hltr-yellow ">" parseInt() provides a second argument: the radix (number of digits). "</mark> [Page 21 ]( zotero://open-pdf/library/items/2BS329KQ?page=21&annotation=XQM7AC63)
        - <mark class="hltr-yellow ">" let num = parseInt("0xAF", 16); // 175 "</mark> [Page 21 ]( zotero://open-pdf/library/items/2BS329KQ?page=21&annotation=LRMP489P)
        - <mark class="hltr-yellow ">" it’s advisable to always include a radix to avoid errors. "</mark> [Page 22 ]( zotero://open-pdf/library/items/2BS329KQ?page=22&annotation=F8A8J64T)
    - <mark class="hltr-orange ">" parseFloat() "</mark> [Page 22 ]( zotero://open-pdf/library/items/2BS329KQ?page=22&annotation=XRD4NPWT)
        - <mark class="hltr-yellow ">" a decimal point is valid the first time it appears, but a second decimal point is invalid and the rest of the string is ignored "</mark> [Page 22 ]( zotero://open-pdf/library/items/2BS329KQ?page=22&annotation=MKU62BPB )
    -

-
  ```js
  Number.parseInt("30px");
  //return '30'
  Number.parseInt("e23");
  //not working
  Number.parseInt("30px", 10);
  //return '30'
  Number.parseFloat("2.5rem");
  //return '2.5'
  ```

-

-
  ```js
  +"";
  //convert a string to number
  ```


## Number Methods
- Check
    -
        - Check if value is Number

    -
      ```js
      Number.isFinite();
      ```

    -
        - Check if a value is Interger

    -
      ```js
      Number.isInteger();
      ```