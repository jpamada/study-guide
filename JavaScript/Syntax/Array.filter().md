#### Definition

**Array.filter()**
Creates a new array containing only elements that pass a condition.

___
#### Syntax

**Syntax 1**
```js
array.filter(
	(element, index, array) => {
	  return condition;
	}
)
```

___
#### Examples

**Example 1**
```js
const arr1 = [
	"a", 10, "b", 20, "c", 30
];

const arr2 = a1.filter(
	(item) => typeof item === "number"
);

// arr2 = [10, 20, 30]
```

___
[[10.01 Array Methods]]