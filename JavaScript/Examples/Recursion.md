#### Examples

**Example 1**
```js
function factorial(n) {
  if (n === 0 || n === 1) {
    return 1;
  }
  return n * factorial(n - 1);
}
```

___
[[04.02 Recursive Function]]