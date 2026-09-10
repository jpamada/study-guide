#### Definition

**Array.find()**
Returns the first element that matches a condition.

___
#### Syntax

**Syntax 1**
```js
array.find(
	(element, index, array) => {
	  return condition;
	}
)
```

___
#### Examples

**Example 1**
```js
const arr = [
	"a", 10, "b", 20, "c", 30
];

const i = arr.find(
	(item) => typeof item === "number"
);

// i = 10
```

___
[[10.01 Array Methods]]