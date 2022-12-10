---
title: DOM
tags: DOM   
started: 2022-12-01 Thu
due: 
modified: 2022-12-06 Tue
status: 
---
[Using the W3C DOM Level 1 Core - Web APIs | MDN](https://developer.mozilla.org/en-US/docs/Web/API/Document_object_model/Using_the_W3C_DOM_Level_1_Core)
## How to use
#### 1. Selector

```js
const guessField = document.querySelector(".guessField");
```

#### 2. Event

```js
guessSubmit.addEventListener("click", checkGuess);
```

#### 3. createElement

```js
resetButton = document.createElement("button");

  resetButton.textContent = "Start new game";
```

#### 4. appendChild

```js
document.body.appendChild(resetButton);
```