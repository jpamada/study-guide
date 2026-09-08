#### Definition

**Promise.catch()**
Handle rejected Promises and errors thrown inside a Promise chain.

___
#### Syntax

**Syntax 1**
```js
promise
  .then((result) => {
    // Success
  })
  .catch((error) => {
    // Error
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
  })
  .catch((error) => {
    console.error("Error:", error);
  });
```

___
[[13.02 Promise Chaining]] | [[13.03 Promise Composition]]