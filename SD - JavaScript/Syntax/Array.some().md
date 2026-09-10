#### Definition

**Array.some()**
Checks if at least one element passes a condition.

___
#### Syntax

**Syntax 1**
```js
array.some(
	(element, index, array) => {
	  return condition;
	}
)
```

___
#### Examples

**Example 1**
```js
function isNumber(value) {
  return typeof value === "number";
}

const a1 = [1, 2, 3];
console.log(a1.some(isNumber)); 
// true

const a2 = [1, "2", 3];
console.log(a2.some(isNumber)); 
// true

const a3 = ["1", "2", "3"];
console.log(a3.some(isNumber)); 
// false
```

___
[[10.01 Array Methods]]