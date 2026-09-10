#### Definition

**Promise.any()**
Returns the first successfully fulfilled Promise. Use when you only need one successful result.

___
#### Syntax

**Syntax 1**
```js
Promise.any([
  promise1,
  promise2,
  promise3,
]);
```

___
#### Examples

**Example 1**
```js
const result = await Promise.any([
  fetchFromServer1(),
  fetchFromServer2(),
  fetchFromServer3(),
]);
```

___
[[13.03 Promise Composition]]