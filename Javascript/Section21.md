# Section 21 Leveling up Functions

#### Function Scope
Variable "visibility" <br>
The location where a variable is defined dictates where we have access to that variable
- functions prioritize the variables inside their scope (closest variable)

#### Block Scope
If the variable is declare inside the block, it only exists inside the block
- `let` and `const` are block scope
-  `var` is a global scrope

#### Lexical Scope
A child function can access to parents functions's variables

#### Function Expressions
You can store functions in variables

```js
  let add = function (x, y) {
    return x + y;
  }
```

#### Higher order functions
Functions that operate on/with other functions.
They can:
- Accept other functions as arguments
```js
function say() {
 console.log('Yes I'm saying sth');
}

function repeat(f) { // Do not execute the function argument
  f();
  f();
}

repeat(say);
```
- Return a function
```js
function range(num1, num2) {
  return function(n) {
    return n >= num1 && n <= num2;
  }
}
```


#### Methods
We can dd functions as properties on obejects. We call them <strong>methods</strong>
```js
const math = {
  multiply: function (x, y) {
    return x * y;
  },
  divide : function (x, y) {
    return x/ y;
  }, 
  square : function (x) {
    return x * x;
  }
}

// Shorthand -> don't need function keyword
const math = {
  multiply(x, y) {
   return x * y;
  }, 
  divide(x, y) {
  return x / y;
}
```

#### `This` in Methods
If `this` is used inside a function inside an object, it refers the object's value of `this`.key.
<br>
But if it is used outside of a object, it refers to `window`
