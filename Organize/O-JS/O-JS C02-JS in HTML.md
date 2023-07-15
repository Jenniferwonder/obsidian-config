---
Title: O-JS C02-JS in HTML
Type: Scope
tags: JavaScript
DateStarted: 2023-07-12
DateModified: 2023-07-14
mindmap-plugin: basic
---

# [[O-JS]] C02-JS in HTML

## Metadata
- Prev:: [[O-JS C01-What is JS]]
- Next:: [[O-JS C03-Language Basics]]

## <mark class="hltr-gray ">" THE `SCRIPT` ELEMENT "</mark> [Page 60 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=60&annotation=DGVYXMWM )
- <mark class="hltr-orange ">" `async` "</mark> [Page 60 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=60&annotation=J2DAXE83)
- <mark class="hltr-orange ">" charset "</mark> [Page 60 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=60&annotation=LX42RWGZ)
- <mark class="hltr-orange ">" crossorigin "</mark> [Page 60 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=60&annotation=DMU5C5VF)
- <mark class="hltr-orange ">" defer "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=R57W98BT)
- <mark class="hltr-orange ">" integrity "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=NZVCF6GM)
- <mark class="hltr-orange ">" src "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=K98LZDHQ)
- <mark class="hltr-orange ">" type "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=2K43E9UP)
- <mark class="hltr-orange ">" two ways to use the `script` element "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=DQ3HK8FY )
   - <mark class="hltr-yellow ">" embed JavaScript code directly into the page "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=XJ375MWA)
   - <mark class="hltr-yellow ">"To include JavaScript from an external file, the `src` attribute is required. "</mark> [Page 61 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=61&annotation=EMKJ4FKJ )
      - ``<script src="example.js"></script> ``
- <mark class="hltr-yellow ">" One of the most powerful and most controversial parts of the script element is its ability to include JavaScript files from outside domains "</mark> [Page 62 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=62&annotation=UK6C8YI4 )
   - <mark class="hltr-yellow ">" Code from an external domain will be loaded and interpreted as if it were part of the page that is loading it. "</mark> [Page 63 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=63&annotation=IYETJBH9 )
   - “`<script src="http://www.somewhere.com/afile.js"></script>`”
   - <mark class="hltr-yellow ">" When including JavaScript files from a different domain, make sure you are the domain owner or the domain is owned by a trusted source. "</mark> [Page 63 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=63&annotation=AXF4DMG4 )

## <mark class="hltr-gray ">" Tag Placement "</mark> [Page 63 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=63&annotation=F8YQVBZP)

## <mark class="hltr-gray ">" Deferred Scripts "</mark> [Page 64 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=64&annotation=93P6J82D)

## <mark class="hltr-gray ">" Asynchronous Scripts "</mark> [Page 64 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=64&annotation=VXAMZSG9)

## <mark class="hltr-gray ">" Dynamic Script Loading "</mark> [Page 65 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=65&annotation=FHKX2UBV)
- <mark class="hltr-orange ">" add script elements "</mark> [Page 65 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=65&annotation=G2X3DDCH)
   - <mark class="hltr-yellow ">" Resources fetched in this fashion will be hidden from browser preloaders "</mark> [Page 65 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=65&annotation=QU2KXEVB)
   - <mark class="hltr-yellow ">" You are not limited to using static script tags to retrieve resources "</mark> [Page 65 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=65&annotation=66RIBDUF )
- <mark class="hltr-orange ">" you can explicitly declare them in the document head: "</mark> [Page 65 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=65&annotation=FFYT4Q6K)
   - “`<link rel="subresource" href="gibberish.js">`”
   - <mark class="hltr-yellow ">" To inform preloaders of the existence of these dynamically requested files "</mark> [Page 65 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=65&annotation=G27BT23W)

## <mark class="hltr-gray ">" Changes in XHTML "</mark> [Page 66 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=66&annotation=Y3TDAWQF)
- <mark class="hltr-orange ">" Extensible HyperText Markup Language, or XHTML "</mark> [Page 66 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=66&annotation=6VY2IR27 )
- <mark class="hltr-yellow ">" a reformulation of HTML as an application of XML "</mark> [Page 66 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=66&annotation=2GFBX3VF )
- <mark class="hltr-yellow ">" The rules for writing code in XHTML are stricter than those for HTML "</mark> [Page 66 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=66&annotation=HM66KQZJ )

## <mark class="hltr-gray ">" Deprecated Syntax "</mark> [Page 67 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=67&annotation=IDA3HCFY)

## <mark class="hltr-gray ">" INLINE CODE VERSUS EXTERNAL FILES "</mark> [Page 68 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=68&annotation=GDNIBRTL)
- <mark class="hltr-yellow ">" it’s generally considered a best practice to include as much JavaScript as possible using external files "</mark> [Page 68 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=68&annotation=J4544YBW )
   - <mark class="hltr-yellow ">" Maintainability "</mark> [Page 68 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=68&annotation=BNF5EWN6)
   - <mark class="hltr-yellow ">" Caching "</mark> [Page 68 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=68&annotation=532FKVLW)
   - <mark class="hltr-yellow ">" Future-proof "</mark> [Page 68 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=68&annotation=6I7BK5RI)

## <mark class="hltr-gray ">" DOCUMENT MODES "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=4HEFIVFR)
- <mark class="hltr-orange ">" doctype switching "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=AFAZPW4D )
   - <mark class="hltr-yellow ">" the primary difference between these two modes is related to the rendering of content with regard to CSS "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=EV6VLGIM )
   - <mark class="hltr-yellow ">" there are also several side effects related to JavaScript "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=F9MYZ4YA )
- <mark class="hltr-orange ">" quirks mode "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=XWDWJW5Z )
   - <mark class="hltr-yellow ">" Quirks mode is achieved in all browsers by omitting the doctype at the beginning of the document. "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=5I7BVWYF )
   - <mark class="hltr-yellow ">" This is considered poor practice "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=W9M8HAZ4 )
   - <mark class="hltr-yellow ">" quirks mode is very different across all browsers "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=XH872MZS )
   - <mark class="hltr-yellow ">" no level of true browser consistency can be achieved without hacks. "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=97E59QGN )
- <mark class="hltr-orange ">" standards mode "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=DS4Z4ZKJ )
   - <mark class="hltr-orange ">" Standards mode is turned on when one of the following doctypes is used: "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=RL5ZTCN9 )
   - ![[C-Professional JavaScript for Web Developers.png|350]]
- <mark class="hltr-orange ">" almost standards mode "</mark> [Page 69 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=69&annotation=K4KQVAYH )

## <mark class="hltr-gray ">" THE `NOSCRIPT` ELEMENT "</mark> [Page 70 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=70&annotation=WNF8YEU9 )
- <mark class="hltr-yellow ">" created to provide alternate content for browsers without JavaScript "</mark> [Page 70 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=70&annotation=YAPFC98M )

## <mark class="hltr-gray ">" SUMMARY "</mark> [Page 71 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=71&annotation=UITHQ7M4 )
- <mark class="hltr-orange ">" src "</mark> [Page 71 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=71&annotation=VJYTI86U )
- <mark class="hltr-yellow ">" elements are interpreted in the order in which they occur on the page "</mark> [Page 71 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=71&annotation=7SG6FZJC )
- <mark class="hltr-yellow ">" so long as defer and async attributes are not used "</mark> [Page 71 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=71&annotation=3PBGAUCQ )
- <mark class="hltr-orange ">" defer "</mark> [Page 71 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=71&annotation=SPDC84S9 )
- <mark class="hltr-orange ">" async "</mark> [Page 71 ]( zotero://open-pdf/library/items/ZK2IJ5LN?page=71&annotation=KE4C7E8X )