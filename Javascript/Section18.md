# Section 18 Javascript Object Literals

#### Creating a Object
We need to designate keys and values
```js
let obj = {
  firstName: 'Mimi',
  lastName: 'Nao',
  age: 14,
  personality: ['caring', 'kind', 'bubbly'],
  graduate: true,
  2012: true
};
```
#### All keys are converted to strings 
You can access the value like below
```js
obj['firstName'] // 'Mimi'
obj.firstName // 'Mimi'
obj[2012] // true
obj['2012'] // true
```

You can also use a variable inside the square brackets to access the values.
```js
let num = 2012;
obj[num] // true
obj.num // undefined
```

