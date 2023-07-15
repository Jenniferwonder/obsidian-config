---
Title: O-JS C09-Proxies and Reflect
Type: Scope
tags: JavaScript
DateStarted: 2023-07-14
DateModified: 2023-07-14
mindmap-plugin: basic
---
# [[O-JS]] C09-Proxies and Reflect
- <mark class="hltr-gray ">" PROXY FUNDAMENTALS "</mark> [Page 2 ]( zotero://open-pdf/library/items/NI9XKU2M?page=2&annotation=2ASUS92A )

	- <mark class="hltr-gray ">" Creating a Passthrough Proxy "</mark> [Page 2 ]( zotero://open-pdf/library/items/NI9XKU2M?page=2&annotation=NT3KLV77)
	
	- <mark class="hltr-gray ">" Defining Traps "</mark> [Page 3 ]( zotero://open-pdf/library/items/NI9XKU2M?page=3&annotation=JNBURUKW)
	
	- <mark class="hltr-gray ">" Trap Parameters and the Reflect API "</mark> [Page 4 ]( zotero://open-pdf/library/items/NI9XKU2M?page=4&annotation=2RBAWSV8)
	
	- <mark class="hltr-gray ">" Trap Invariants "</mark> [Page 6 ]( zotero://open-pdf/library/items/NI9XKU2M?page=6&annotation=ZTUENV9J)
	
	- <mark class="hltr-gray ">" Revocable Proxies "</mark> [Page 7 ]( zotero://open-pdf/library/items/NI9XKU2M?page=7&annotation=RMRDAZSW)
	
	- <mark class="hltr-gray ">" Utility of the Reflect API "</mark> [Page 7 ]( zotero://open-pdf/library/items/NI9XKU2M?page=7&annotation=SYN5F7E9)
	
		- <mark class="hltr-gray ">" Reflect API vs. Object API "</mark> [Page 8 ]( zotero://open-pdf/library/items/NI9XKU2M?page=8&annotation=9H8VA83Y)
		
		- <mark class="hltr-gray ">" Status Flags "</mark> [Page 8 ]( zotero://open-pdf/library/items/NI9XKU2M?page=8&annotation=HS4NWKH6)
		
		- <mark class="hltr-gray ">" Supplanting Operators with First-Class Functions "</mark> [Page 9 ]( zotero://open-pdf/library/items/NI9XKU2M?page=9&annotation=DXRJIH8Q)
		
		- <mark class="hltr-gray ">" Safe Function Application "</mark> [Page 9 ]( zotero://open-pdf/library/items/NI9XKU2M?page=9&annotation=55L737ET)
	
	- <mark class="hltr-gray ">" Proxying a Proxy "</mark> [Page 9 ]( zotero://open-pdf/library/items/NI9XKU2M?page=9&annotation=CIMV6S94)
	
	- <mark class="hltr-gray ">" Proxy Considerations and Shortcomings "</mark> [Page 10 ]( zotero://open-pdf/library/items/NI9XKU2M?page=10&annotation=LWT3XF4E)
	
		- <mark class="hltr-gray ">" ’this’ Inside a Proxy "</mark> [Page 10 ]( zotero://open-pdf/library/items/NI9XKU2M?page=10&annotation=H8A4D2IX)
		
		- <mark class="hltr-gray ">" Proxies and Internal Slots "</mark> [Page 11 ]( zotero://open-pdf/library/items/NI9XKU2M?page=11&annotation=H98J49PD)

- <mark class="hltr-gray ">" PROXY TRAPS AND REFLECT METHODS "</mark> [Page 11 ]( zotero://open-pdf/library/items/NI9XKU2M?page=11&annotation=XEAQ52EE)

	- <mark class="hltr-gray ">" get() "</mark> [Page 11 ]( zotero://open-pdf/library/items/NI9XKU2M?page=11&annotation=32UP4538)
	
	- <mark class="hltr-gray ">" set() "</mark> [Page 12 ]( zotero://open-pdf/library/items/NI9XKU2M?page=12&annotation=3UWH36PP)
	
	- <mark class="hltr-gray ">" has() "</mark> [Page 13 ]( zotero://open-pdf/library/items/NI9XKU2M?page=13&annotation=PL9Z956C)
	
	- <mark class="hltr-gray ">" defineProperty() "</mark> [Page 14 ]( zotero://open-pdf/library/items/NI9XKU2M?page=14&annotation=FMP7TDBZ)
	
	- <mark class="hltr-gray ">" getOwnPropertyDescriptor() "</mark> [Page 15 ]( zotero://open-pdf/library/items/NI9XKU2M?page=15&annotation=2LLYLLMQ)
	
	- <mark class="hltr-gray ">" deleteProperty() "</mark> [Page 16 ]( zotero://open-pdf/library/items/NI9XKU2M?page=16&annotation=C82YHIGV)
	
	- <mark class="hltr-gray ">" ownKeys() "</mark> [Page 17 ]( zotero://open-pdf/library/items/NI9XKU2M?page=17&annotation=YDQZVJFX)
	
	- <mark class="hltr-gray ">" getPrototypeOf() "</mark> [Page 17 ]( zotero://open-pdf/library/items/NI9XKU2M?page=17&annotation=LZSLDHNF)
	
	- <mark class="hltr-gray ">" setPrototypeOf() "</mark> [Page 18 ]( zotero://open-pdf/library/items/NI9XKU2M?page=18&annotation=T7TKS2BZ)
	
	- <mark class="hltr-gray ">" isExtensible() "</mark> [Page 19 ]( zotero://open-pdf/library/items/NI9XKU2M?page=19&annotation=A73SK3TG)
	
	- <mark class="hltr-gray ">" preventExtensions() "</mark> [Page 20 ]( zotero://open-pdf/library/items/NI9XKU2M?page=20&annotation=V6T62NFV)
	
	- <mark class="hltr-gray ">" apply() "</mark> [Page 20 ]( zotero://open-pdf/library/items/NI9XKU2M?page=20&annotation=AI4IAB4J)
	
	- <mark class="hltr-gray ">" construct() "</mark> [Page 21 ]( zotero://open-pdf/library/items/NI9XKU2M?page=21&annotation=T692Y896)

- <mark class="hltr-gray ">" PROXY PATTERNS "</mark> [Page 22 ]( zotero://open-pdf/library/items/NI9XKU2M?page=22&annotation=LH7ZB4HZ)

	- <mark class="hltr-gray ">" Tracking Property Access "</mark> [Page 22 ]( zotero://open-pdf/library/items/NI9XKU2M?page=22&annotation=SPKFLNVV)
	
	- <mark class="hltr-gray ">" Hidden Properties "</mark> [Page 23 ]( zotero://open-pdf/library/items/NI9XKU2M?page=23&annotation=B9YBDST2)
	
	- <mark class="hltr-gray ">" Property Validation "</mark> [Page 23 ]( zotero://open-pdf/library/items/NI9XKU2M?page=23&annotation=SAE3X78X)
	
	- <mark class="hltr-gray ">" Function and Constructor Parameter Validation "</mark> [Page 24 ]( zotero://open-pdf/library/items/NI9XKU2M?page=24&annotation=GMM52NHU)
	
	- <mark class="hltr-gray ">" Data Binding and Observables "</mark> [Page 25 ]( zotero://open-pdf/library/items/NI9XKU2M?page=25&annotation=VL3HLKJJ)