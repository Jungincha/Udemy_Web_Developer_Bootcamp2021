# Newer Javascript Features

#### Default Params
Make sure you put the default parameter at the end of the barckets
```js
function mult(a, b = 1) {
  return a * b;
}
```

#### Spread syntax
`spread` allows an interable such as an array expression or string to be expanded in places
```js
let arr = [1,2,3,4]

console.log(...arr)
// 1 2 3 4
```

#### Spread with Array literals
Create a new array using an existing array. Spreads the elements from on array into a new array
```js
const num1 = [1,2,3,4];
const num2 = [5,6,7,8];

[...num1, ...num2];
// [1,2,3,4,5,6,7,8]
```

#### Spread in Object literals
Create a new object using an existing object.
```js
const obj = {name: 'Bokhee', age: 1};

let newObj = {...obj, breed: 'Norway forest'};
```

#### Rest Parameter
It allows a function to accept an indefinite number of arguments as an array
```js
function num(...nums) {
  console.log(nums);
}

num(1,2,3,4) // [1, 2, 3, 4]
 ```
#### Destructuring Arrays
It's a Js expression that makes it possible to unpack values from arrays. or properties from objects, into distinct variables
```js
const num = [1, 2, 3, 4, 5, 6, 7];

const [one, two, ...restNumbers] = num;

// one => 1
// two => 2
// restNumbers => [3, 4, 5, 6, 7]
```
#### Destructuring Objects
```js
const catInfo = {
  name: 'bebe',
  age: 7,
  gender: 'male'
}

const {name, age, gender} = catInfo;
// name => 'bebe'
// age => 7
// gender => 'male
```

#### Destructuring Parameter
```js
const catInfo = {
  name: 'bebe',
  age: 7,
  gender: 'male'
}

const read = ({name, gender}) => {
  return `${name} is a ${gender} cat.`;
}

read(catInfo); // 'bebe is a male cat.' 
```
