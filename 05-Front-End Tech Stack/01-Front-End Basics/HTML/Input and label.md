---
title: Input
tags: HTML
started: 2022-12-06 Tue
due:
modified: 2022-12-06 Tue
status:
---
>[The Input (Form Input) element - HTML | MDN](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input)
## Questions
- `input type - button` and `button element`?
## How to use?
```html
<label for="name">Name (4 to 8 characters):</label>
<input type="text" id="name" name="name" required minlength="4" maxlength="8" size="10">
```
## JS Method
```js
guessField.disabled = false;
guessSubmit.disabled = false;
guessField.focus();
guessField.value = "";
```
## Basics
- type
- id
- name
- minlength
- maxlength
- min
- max
- value
- required
- disabled