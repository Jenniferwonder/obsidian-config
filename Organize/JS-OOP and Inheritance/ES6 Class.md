---
Title: ES6 Class
tags:
DateStarted: 2022-12-02
due:
DateModified: 2022-12-02
status:
---

## Learning Resources

[Classes - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
[Classes in JavaScript - Learn web development | MDN](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Classes_in_JavaScript)

## [Classes and constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Classes_in_JavaScript#classes_and_constructors)

```js
class Person {
	name;
	constructor(name) {
		this.name = name;
	}
	introduceSelf() {
		console.log(`Hi! I'm ${this.name}`);
	}
}
```

### [Omitting constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Classes_in_JavaScript#omitting_constructors)

If you don't need to do any special initialization, you can omit the constructor, and a default constructor will be generated for you.

## [Inheritance](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Classes_in_JavaScript#inheritance)

```js
class Professor extends Person {
	teaches;
	constructor(name, teaches) {
		super(name);
		this.teaches = teaches;
	}
	introduceSelf() {
		console.log(
			`My name is ${this.name}, and I will be your ${this.teaches} professor.`
		);
	}
	grade(paper) {
		const grade = Math.floor(Math.random() * (5 - 1) + 1);
		console.log(grade);
	}
}
```

## [Encapsulation](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Classes_in_JavaScript#encapsulation)

```js
class Student extends Person {
	#year;
	constructor(name, year) {
		super(name);
		this.#year = year;
	}
	introduceSelf() {
		console.log(`Hi! I'm ${this.name}, and I'm in year ${this.#year}.`);
	}
	canStudyArchery() {
		return this.#year > 1;
	}
}
```
