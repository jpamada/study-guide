#### Definition

**AbortController**
Cancellation is used when you want to stop an asynchronous operation that is no longer needed.

___
#### Syntax

**Syntax 1**
```js
const controller = 
	new AbortController();

operation({
  signal: controller.signal,
});

controller.abort();
```

___
#### Examples

**Example 1**
```js
const controller = 
	new AbortController();

fetch("/api/users", {
  signal: controller.signal,
});

controller.abort();
```

___
[[13.04 Cancellation]]
