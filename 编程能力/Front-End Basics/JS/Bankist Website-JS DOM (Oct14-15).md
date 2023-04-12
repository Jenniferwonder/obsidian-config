---
title: Bankist Website-JS DOM (Oct14-15)
tags: 
status: 
started: 
due: 
aliases: 
---
## Project Overview
An online bank landing page
#### TIME

| **Start Time** | Oct 14-15 |

| --- | --- |

| **Due Time** | Oct 15 |
| **Total Time Spent** | 2 Days>  |
| **New Issues Added** | 

- 
 |
#### SCOPE
| #### G2- JS Master
 | 
- Modal 
- Smooth Scroll (button, navigation)
- Tabbed Components (标签页)
- Menu Fading Animation
- Sticky Navbar
- **Reveal Elements on Scrolling**
- Image Lazy Loading (图片懒加载)
- Slider (轮播图)
 |
| --- | --- |
## Modal
#### HTML& CSS
- .modal
- .overlay
- .hidden
- .btn--show-modal
- .btn--close-modal
#### JS DOM
- Event
   - .addEventListener('click', <closeModal>);
   - 'keydown'
      - document.addEventListener('keydown', function (e) {
  if (e.key === 'Escape' && !modal.classList.contains('hidden')) {closeModal();}});
- Class
   - .classList.add('hidden')
   - .classList.remove('hidden')
   - .classList.contains('hidden')
- Selector
   - document.querySelector('')
   - document.querySelectorAll('')
## Navigation
#### HTML& CSS
- .nav
- .nav__logo, `#logo`
- .nav__links
- .nav__link
- `#section`--1, 2, 3
### Smooth Scrolling
#### JS DOM
- Attribute
   - const **id** = e.target.getAttribute('href')
- Selector
   - document.querySelector(**id/ #...**)
- Scrolling methods
   - `<targetEl>`**.scrollIntoView**({behavior: 'smooth'})
### Menu Fading Animation
#### JS DOM
- DOM traversing
   - const link = e.target;
   - const siblings = link.closest('.nav').querySelectorAll('.nav__link');
   - const logo = link.closest('.nav').querySelector('img');
- Passing "argument" into Event handler
   - const handleHover = function (e) {...if (el !== link) el.style.opacity **= this**;}
   - nav.addEventListener('mouseover', handleHover**.bind**(0.5));
### Sticky Navigation
- **.getBoundingClientRect()**.height
- **IntersectionObserver** API
   - new IntersectionObserver(obsCallback, obsOptions)
## Tabbed Components
#### HTML& CSS
- .operations__tab-container
- .operations__tab
   - .operations__tab--1, 2, 3
   - .operations__tab--active
   - data-tab="1/ 2/ 3"S
- .operations__content
   - .operations__content--1, 2, 3
      - `.operations__content--${clicked.**dataset.tab**}`
   - .operations__content--active
#### JS DOM
- Event delegation 
   - tabsContainer**.addEventListener**()
- DOM traversing
   - const clicked = e.target**.closest**('.operations__tab');
## Scrolling Effects
### Reveal Elements on Scrolling
### Image Lazy Loading 
### 
