# Section 17 Javascript Array

#### Arrary Random Access

- Accessing by an index number
```js
let names = ['Mina', 'Somi', 'Ahmi', 'Bomi'];
names[0] // Mina
```

- `Push` & `Pop`, `Shift` & `Unshift`
```js
names.push('Nami');
// ['Mina', 'Somi', 'Ahmi', 'Bomi', 'Nami']

names.pop();
// ['Mina', 'Somi', 'Ahmi', 'Bomi']

name.shift();
// ['Somi', 'Ahmi', 'Bomi']

name.unshift('Innie');
// ['Innie', 'Somi', 'Ahmi', 'Bomi']
```

- `Concat`, `indexOf`, `includes` & `reverse`
- `Slice` & `Splice`

#### Reference Types & Equality Testing
When you make an array, you are storing that array in a specific reference(address).
<br>
Let's say you made an array like below.
```js
let num = [1,2,3];
```
`num` is stored in some address. So eventhough there is another array looks similar, you can't do a equality test by comparing the arrays.
```js
let number = [1,2,3];
num === number; // false --> different address
```
And if you assign a new variable to the main array like below, 
```js
let number = num; 
// number --> [1,2,3]
```
`num` and `number` arrays are pointing at the exactly same address.(Same pointer). So if you change one array, the other one will change too.
```js
num.push(4);
// number --> [1,2,3,4]
```

#### Arrays + Const
You can't change a `string` or `number` `const`. But with Arrays you can still modify the array with functions unless you designate a new array at the same variable.
```js
const num = [1,2,3];
num.push(4);
// num --> [1,2,3,4]
```

#### Multi-Dimensional Arrays
```js
let multiArrays = [
  [o, o, x],
  [x, null, x],
  [o, x, null]
];
```
