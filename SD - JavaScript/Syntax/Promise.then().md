#### Definition

**Promise.then()**
Returns a new Promise, allowing the next step to wait for a returned Promise to settle.

___
#### Syntax

**Syntax 1**
```js
promise
  .then((result) => {
    return nextPromise(result);
  })
  .then((result) => {
    return anotherPromise(result);
  });
```

___
#### Examples

**Example 1**
```js
fetchUser()
  .then((user) => {
    return fetchPosts(user.id);
  })
  .then((posts) => {
    console.log(posts);
  });
```

___
[[13.02 Promise Chaining]]