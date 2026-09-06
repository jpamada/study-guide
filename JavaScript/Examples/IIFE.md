**Example 1**
```js
(function () {
  // Do something
})();
```

**Example 2**
```js
const value = (function () {
  // Do something
  return someValue;
})();
```

**Example 3**
```js
(() => {
  console.log("Hello");
})();
```

**Example 4**
```js
const config = (() => {
  const apiUrl = "https://example.com";

  return {
    apiUrl,
  };
})();
```

___
[[04.03 IIFE]]