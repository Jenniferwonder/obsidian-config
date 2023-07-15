---
Title: O-JS C04-Variables, Scope, Memory
Type: Scope
tags: JavaScript
DateStarted: 2023-07-13
DateModified: 2023-07-14
mindmap-plugin: basic
---

# [[O-JS]] C04-Variables, Scope, Memory

## <mark class="hltr-gray ">" PRIMITIVE AND REFERENCE VALUES "</mark> [Page 1 ]( zotero://open-pdf/library/items/777VEPFY?page=1&annotation=M6CPPAQ8 )
- <mark class="hltr-orange ">" Primitive values "</mark> [Page 1 ]( zotero://open-pdf/library/items/777VEPFY?page=1&annotation=IT8YHYTZ)
    - <mark class="hltr-orange ">" six primitive types "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=3DJS2H4R)
        - <mark class="hltr-orange ">" Undefined, Null, Boolean, Number, String, and Symbol "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=2NXN4HBB)
    - <mark class="hltr-yellow ">" These variables are said to be accessed by value, because you are manipulating the actual value stored in the variable. "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=UMTVM7XE)
- <mark class="hltr-orange ">" Reference values "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=Z98XHI53)
    - <mark class="hltr-yellow ">" objects stored in memory. "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=NXCRTCJR)
    - <mark class="hltr-yellow ">" When you manipulate an object, you’re really working on a reference to that object rather than the actual object itself "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=Y8ITK2AN)
- <mark class="hltr-gray ">" Dynamic Properties "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=PMXIWGYR)
    - <mark class="hltr-orange ">" reference values "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=U5P3W6SX)
        - <mark class="hltr-yellow ">" you can add, change, or delete properties and methods at any time "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=FIZ2YTPL)
    - <mark class="hltr-orange ">" Primitive values "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=DL6JSJAY)
        - <mark class="hltr-yellow ">" can’t have properties added to them even though attempting to do so won’t cause an error. "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=RJGZB524)
    - <mark class="hltr-orange ">" primitive literal form "</mark> [Page 2 ]( zotero://open-pdf/library/items/777VEPFY?page=2&annotation=FPCIM9TN)
- <mark class="hltr-gray ">" Copying Values "</mark> [Page 3 ]( zotero://open-pdf/library/items/777VEPFY?page=3&annotation=4I4NIZMA)
- <mark class="hltr-gray ">" Argument Passing "</mark> [Page 3 ]( zotero://open-pdf/library/items/777VEPFY?page=3&annotation=L64HPRQ9)
- <mark class="hltr-gray ">" Determining Type "</mark> [Page 5 ]( zotero://open-pdf/library/items/777VEPFY?page=5&annotation=SH9URHH6)

## <mark class="hltr-gray ">" EXECUTION CONTEXT AND SCOPE "</mark> [Page 6 ]( zotero://open-pdf/library/items/777VEPFY?page=6&annotation=IIHW6HAJ)
- [[O-JS Scope-作用域]]
    - <mark class="hltr-gray ">" Scope Chain Augmentation "</mark> [Page 8 ]( zotero://open-pdf/library/items/777VEPFY?page=8&annotation=92V2RUYU)
- [[O-JS Variables]]
    - <mark class="hltr-gray ">" Function Scope Declaration Using var "</mark> [Page 9 ]( zotero://open-pdf/library/items/777VEPFY?page=9&annotation=BXPR6RKC)
    - <mark class="hltr-gray ">" Block Scope Declaration Using let "</mark> [Page 11 ]( zotero://open-pdf/library/items/777VEPFY?page=11&annotation=454XNBUM)
    - <mark class="hltr-gray ">" Constant Declaration Using const "</mark> [Page 12 ]( zotero://open-pdf/library/items/777VEPFY?page=12&annotation=RV8JVWYD)
    - <mark class="hltr-gray ">" Identifier Lookup "</mark> [Page 13 ]( zotero://open-pdf/library/items/777VEPFY?page=13&annotation=62NCXD2X)

## <mark class="hltr-gray ">" GARBAGE COLLECTION "</mark> [Page 14 ]( zotero://open-pdf/library/items/777VEPFY?page=14&annotation=5E6RTDVT)
- <mark class="hltr-gray ">" Mark-and-Sweep "</mark> [Page 15 ]( zotero://open-pdf/library/items/777VEPFY?page=15&annotation=E7RH78YN)
- <mark class="hltr-gray ">" Reference Counting "</mark> [Page 15 ]( zotero://open-pdf/library/items/777VEPFY?page=15&annotation=3Z5S8B59)
- <mark class="hltr-gray ">" Performance "</mark> [Page 16 ]( zotero://open-pdf/library/items/777VEPFY?page=16&annotation=3S2S5IHX)
- <mark class="hltr-gray ">" Managing Memory "</mark> [Page 17 ]( zotero://open-pdf/library/items/777VEPFY?page=17&annotation=ZCQRAGP8)
    - <mark class="hltr-gray ">" Performance Boosts with const and let Declarations "</mark> [Page 18 ]( zotero://open-pdf/library/items/777VEPFY?page=18&annotation=TIYHTYRX)
    - <mark class="hltr-gray ">" Hidden Classes and the delete Operation "</mark> [Page 18 ]( zotero://open-pdf/library/items/777VEPFY?page=18&annotation=SJS2JDHM)
    - <mark class="hltr-gray ">" Memory Leaks "</mark> [Page 19 ]( zotero://open-pdf/library/items/777VEPFY?page=19&annotation=8AD54VW7)
    - <mark class="hltr-gray ">" Static Allocation and Object Pools "</mark> [Page 20 ]( zotero://open-pdf/library/items/777VEPFY?page=20&annotation=FB88CPI7)