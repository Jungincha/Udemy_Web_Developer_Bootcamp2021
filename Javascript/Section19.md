# Section 19 Repeating struff with loops

#### Basic For loop
```js
for (let i = 0; i <= 3; i++) {
  console.log(i);
  // 0, 1, 2, 3
}
```

#### The perils of infinite loops 
```js
for (let i = 100; i >= 0; i++){
  console.log(i);
  // it will crash since there is no limit
  // always check the limit and the range
}
```

#### While loop
```js
const SECRET = 'BabyHippo';

let guess = prompt('Enter the secret code');

while (guess !== SECRET) {
  guess = prompt("Enter the secret code");
}
console.log('Congrats you got the secret');
```

#### For...of loop
A nice and easy way of iterating over arrays (or other iterable objects)
```js
const subreddits = ['books', 'cat', 'pics', 'dog', 'bird'];

for (let i = 0; i < subreddits.length; i++) {
  console.log(subreddits[i]);
}

for (let sub of subreddits) {
  console.log(sub);
}
```

### For...in loop
iterates Object's key

### Object functions
- Object.keys(objName)
- Object.values(objName)
- Object.entries(objName) --> Gives you the nested array of keys and values
