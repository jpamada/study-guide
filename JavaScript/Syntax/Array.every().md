#### Definition

****

___
#### Syntax

**Syntax 1**
```js
array.every(
	(element, index, array) => {
	  return condition;
	}
);
```

___
#### Examples

**Example 1**
```js
function isNumber(value) {
  return typeof value === "number";
}

const a1 = [1, 2, 3];
console.log(a1.every(isNumber)); 
// true

const a2 = [1, "2", 3];
console.log(a2.every(isNumber)); 
// false
```

___
[[09.01 Array Methods]]