#### Definition

**Promise Chaining**
Promise chaining is used when asynchronous operations need to happen one after another.

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
  })
  .catch((error) => {
    // Handle error
  });
```

___
#### Examples

**Normal Chaining**
```js
fetchUser()
  .then((user) => {
    return fetchPosts(user.id);
  })
  .then((posts) => {
    console.log(posts);
  })
  .catch((error) => {
    console.error(error);
  });
```

**Chaining After Promise.catch()**
```js
doSomething()
  .then(() => {
    throw new Error("Error Message");
  })
  .catch((error) => {
    console.error(error.message);
  })
  .then(() => {
    console.log("This still runs");
  });
```

___
[[13.02 Promise Chaining]]