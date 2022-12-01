---
title: Array
tags: JS
started: 2022-12-01 Thu
due: 
modified: 2022-12-01 Thu
status: 
number headings: auto, first-level 4, max 6, 1.1.
---
## Array Methods
#### 1. Return array index
##### 1.1. based on value

```js
.indexOf 
//Get the index of an element
```

##### 1.2. based on test condition

```js
.findIndex(arr => acc.username === currentAcc.username)
//return the index of the first element that matches the condition
```

#### 2. Return an array element based on test condition

```js
.find (mov => mov < 0) 
//return the first element that satisfies the condition
.at(0)
//similar to 'arr[0]'
```

#### 3. Return a computed value

```js
.reduce(function(sum, `loopingElement`, index, arr) { }, `0/initial value`) 
.reduce((sum, `loopingElement`) => sum + `looEle`, `0/initial value`); 
//to get the max/min number or sum in an array
```

#### 4. Mutate original array
##### 4.1. Add to original

```js
.push()
//Add element at the end of array
.unshift
//Add element at the start of array
.fill(1, 2, 5)  
//fill an array with the specified element 1 from index 2 to 5  
```

##### 4.2. Remove from original  

```js
.pop  
//Remove the last element of array  
.shift  
//Remove the first element of array  
.splice(1, 2)  
//To delete 2 elements from index position 1 from an array  
```

##### 4.3. Order

```JS
.reverse()  
//To reverse order of elements in an array  
.sort( )  
//sort an array alphabetically, treating element as a string  
.sort((a, b) => a-b);/ {if (a > b) return 1; else return -1;});  
//to put number in an ascending order  
```

#### 5. Return a new array  
##### 5.1. Computed from original  

```js
.map(function `arr * 2`)  
```

##### 5.2. Filtere using conditional  

```js
.filter(function`arr > 2`)  
//return a new array of all elements that satisfy the condition 
``` 

##### 5.3. Portion of original  

```js
.slice(4)  
//to extract the elements of a string starting from index 4 position  
.slice(4,7)  
//to extract the elements from index 4 to 7  
.slice(-1)  
//to get the last character of a string  
```

##### 5.4. Add original to other  

```js
.concat(`newArray`)  
//To combine 2 arrays into 1 new array  
//similar to [...arr, ...arr2]  
```

##### 5.5. Flattening the original  

```js
.flat(1/2) (ES2019)  
//to convert nested array into one big array  
.flatMap(function)  
//combine "map" and "flat" method to flat a map one level deep  
```

##### 5.6. Spread  

```js
...[`array`]  
//to spread element in iterables  
```

##### 5.7. Rest  

```js
...[`array`]  
//to put the rest elements into the array  
```

#### 6. Create a new array  

```js
new Array(1, 2, 3)  
//return [1, 2, 3]  
new Array(3)  
//return empty array with 3 empty elements  
.fill(1, 2, 5)  
//fill an array with the specified value 1 from index 2 to 5 
``` 

#### 7. Convert array-like structure into an array  🟨

```js
Array.from({ length: 3}, () => 1)  
//return [1, 1, 1]  
Array.from({ length: 3}, (_, i) => i+1)  
//return [1, 2, 3]  
Array.from(document.querySelectorAll('.<className>'), function)  
//create an array of element with the same html className 
```

#### 8. Know if array includes  
##### 8.1. based on value  

```js
.includes()  
//Check if an element is in the array 
``` 

##### 8.2. based on test condition  

```js
.some(mov => mov > 0)  
//To get an array of the elements in an array that match the condition  
//return "true" if some elements in the array match the condition  
.every(mov => mov >0)  
//return "true" if every element in the array matches the condition
```

#### 9. Destructuring  

```js
//store array elements into new variables  
[`varName`] = array  
```