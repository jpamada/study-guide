**Example 1**
Both let/const is in temporal dead zone.
```js
console.log(name); 
// ReferenceError

let name = "John";
```

___
[[01.02 Variable Hoisting]]