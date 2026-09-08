#### Definition

**Promise.allSettled()**
Waits until all Promises finish, whether they succeed or fail.

___
#### Syntax

**Syntax 1**
```js
Promise.allSettled([
  promise1,
  promise2,
  promise3,
]);
```

___
#### Examples

**Example 1**
```js
const results = await Promise.allSettled([
  fetchUser(),
  fetchPosts(),
  fetchComments(),
]);

/*
[
  {
    status: "fulfilled",
    value: { id: 1 },
  },
  {
    status: "rejected",
    reason: Error("Failed"),
  },
];
*/
```

___
[[13.03 Promise Composition]]