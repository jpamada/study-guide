#### Examples

**Example 1**
The `name` variable have empty string therefore it is a falsy.
```js
const name = "";
const displayName = 
  name || "Guest";

console.log(displayName); 
// "Guest"
```

___
[[05.02 Fallback Operators]]