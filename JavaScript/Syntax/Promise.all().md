#### Definition

**Promise.all()**
Waits for all Promises to succeed.

___
#### Syntax

**Syntax 1**
```js
Promise.all([
  promise1,
  promise2,
  promise3,
]);
```

___
#### Examples

**Example 1**
```js
const [user, posts] = await Promise.all([
  fetchUser(),
  fetchPosts(),
]);
```

___
[[13.03 Promise Composition]]