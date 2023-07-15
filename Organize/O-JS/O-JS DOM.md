---
Type: Scope
Title: O-JS DOM
tags: JavaScript
DateStarted: 2022-12-01
DateModified: 2023-07-14
status:
aliases: DOM
mindmap-plugin: basic
---

# [[O-JS]] DOM

## Metadata
- Up:: [[O-JS]]
- Related:: [[O-JS C01-What is JS]]

## Reference
- [Using the W3C DOM Level 1 Core - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_object_model/Using_the_W3C_DOM_Level_1_Core)

## Overview
- ![[Pasted image 20230310114615.png]]

## <mark class="hltr-gray ">" The Document Object Model "</mark> [Page 54 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=54&annotation=HGBVMQVE )
- <mark class="hltr-yellow ">" The Document Object Model (DOM) is an application programming interface (API) for XML that was extended for use in HTML. "</mark> [Page 54 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=54&annotation=MSNC8X4K )
- <mark class="hltr-gray ">" Why the DOM Is Necessary "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=Y9CXZ4RU)
    - <mark class="hltr-orange ">" World Wide Web Consortium (W 3 C) "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=RJG5RX9Q )
- <mark class="hltr-gray ">" DOM Support in Web Browsers "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=XDVD4GDD )
- <mark class="hltr-yellow ">" For web browsers, however, the DOM has been implemented using ECMAScript and now makes up a large part of the JavaScript language. "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=4WT7DGZZ)

## <mark class="hltr-gray ">" DOM Levels "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=E4EKLDJP)
- <mark class="hltr-orange ">" DOM Level 1 "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=NDUZFUVV)
    - <mark class="hltr-yellow ">" the DOM Core "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=YSJQWCTR)
        - Element
            -
                - createElement

            - 
              ```js  
              resetButton = document.createElement("button");  
              resetButton.textContent = "Start new game";  
              ```

            -
                - appendChild

            -

              ```js
              document.body.appendChild(resetButton);
              ```

    - <mark class="hltr-yellow ">" DOM HTML "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=6ML3UFET)
        - Selector
            -
                - `document.querySelector`
                - `document.getElementById`

            - 
              ```js  
              const guessField = document.querySelector(".guessField");  
              ```

        - ClassList
            - `document.classList.add/toggle/remove`
- <mark class="hltr-orange ">" DOM Level 2 "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=KZBEV8JR)
    - <mark class="hltr-yellow ">" DOM views "</mark> [Page 55 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=55&annotation=T89H4FY3)
    - <mark class="hltr-yellow ">" DOM events "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=V8BVSIUC)
        - Event

            -

              ```js
              guessSubmit.addEventListener("click", checkGuess);
              ```

    - <mark class="hltr-yellow ">" DOM style "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=MFUZT29S)
    - <mark class="hltr-yellow ">" DOM traversal and range "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=ESH3YUZY)
- <mark class="hltr-orange ">" DOM Level 3 "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=YAMRL4ZA)
    - <mark class="hltr-yellow ">" DOM Load and Save "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=7H4ZKPAT )
- <mark class="hltr-orange ">" DOM Living Standard "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=CMBKI8AP )

## <mark class="hltr-gray ">" Other DOMs "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=KFGXNDZK )
- <mark class="hltr-orange ">" The languages in the following list are XML-based, and each DOM adds methods and interfaces unique to a particular language "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=85JJGEYH)
    - <mark class="hltr-yellow ">" Scalable Vector Graphics (SVG) "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=M96W5C2R)
    - <mark class="hltr-yellow ">" Mathematical Markup Language (MathML) "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=RBCEB999)
    - <mark class="hltr-yellow ">" Synchronized Multimedia Integration Language (SMIL) "</mark> [Page 56 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=56&annotation=6IWPCU35 )

## How to use