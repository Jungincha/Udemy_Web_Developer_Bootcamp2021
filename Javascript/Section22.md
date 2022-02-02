# Section 22 Callbacks & Array Methods

#### callback
A function which is to be executed after another function has finished execution. Any function that is passed as an argument to another function so that it can be executed in that other function is called as a call back function.

#### forEach Method
Accepts a callback function. Calls the function once per element in the array.

```js
let arr = [1,2,3,4]

arr.forEach(function (el) {
  console.log(el);
})
// 1 
// 2
// 3
// 4
```

#### Map 
Creates a new array with the results of calling a callback on every element in the array

#### Arrow functions
```js
const add = function (x, y) {
  return x + y;
}

const add = (x, y) => {
  return x + y; 
}
```
#### setTimeout & setInterval
`setTimeout` executes the callback function after ---ms. 
```js
setTimeout(() => {
  console.log(Math.floor(Math.random() * 6) + 1)
}, 3000)
```
`setInterval` executes the callback function every ---ms.
```js
const id = setInterval(() => {
  console.log(Math.floor(Math.random() * 6) + 1)
}, 2000)
```

#### Filter method
`filter` method filters out the elements with specific condition and make them into an array.
```js
let arr = [1, 2, 3, 4];

let oddNum = arr.filter(num => num % 2 === 0);
```

#### some & every
`some` returns true if any of the array elements pass the test function
<br>
`every` tests whether all elements in the array pass the provided function.

#### reduce()
`reduce` sums up an array to a element
```js
const arr = [1, 2, 3, 4];

arr.reduce((sum, el) => sum + el);
```
`reduce` sorts out an element
```js
const arr = [3, 5, 1, 10, 4];

arr.reduce((bigNum, curNum) => {
  if (bigNum < curNum) return curNum
  return bigNum;
});
```

#### Arrow functions & `this`
`this` reacts different in arrow function
