#### Examples

**Example 1**
The `counter` did not reset
```js
function createCounter() {
  let count = 0;

  return function () {
    count++;
    return count;
  };
}

const counter = createCounter();

console.log(counter()); // 1
console.log(counter()); // 2
console.log(counter()); // 3
```

**Example 2**
You can create multiple scope.
```js
const counter1 = createCounter();
const counter2 = createCounter();

console.log(counter1) // 0
console.log(counter2) // 0
```

___
#### Steps

**01 Create a Function**
The `count` variable does not exist yet because the function is not yet called.
```js
function createCounter() {
  let count = 0;
  // ...
}
```

**02 Call the Function**
JavaScript now have `count`
```js
const counter = createCounter();
```

**03 Runs the Inner Function**
The inner function has access to the outer scope variable `count`.
```js
function increment() {
  count++;
  return count;
}
```

**04 Returns the Updated Count**
The `counter` variable now holds the returned incremented `count.`
```js
const counter = createCounter();
```

**05 Call The Variable**
The variable now holds the function and can remember the same variable.
```js
counter(); // 1
counter(); // 2
counter(); // 3
```

___
[[04.04 Closures]]