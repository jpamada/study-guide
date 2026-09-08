#### Definition

**Promise**
A Promise represents the eventual success or failure of an asynchronous operation.

___
#### Syntax

**Syntax 1**
```js
new Promise((resolve, reject) => {
  // asynchronous operation
});
```

___
#### Examples

**Example 1**
```js
const promise = new Promise(
	(resolve, reject) => {
	  const success = true;

	  if (success) {
	    resolve("Data loaded");
	    
	  } else {
	    reject(
		    new Error("Error Message");
		  );
	  }
	}
);
```

___
[[13.01 Promises]]
