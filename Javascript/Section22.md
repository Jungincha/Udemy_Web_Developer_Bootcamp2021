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
