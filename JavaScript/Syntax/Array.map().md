#### Definition

**Array.map()**
Creates a new array by transforming every element.

___
#### Syntax

**Syntax 1**
```js
array.map(
	(element, index, array) => {
	  return newValue;
	}
)
```

___
#### Examples

**Example 1**
```js
const arr1 = ["a", "b", "c"];

const arr2 = a1.map(
	(item) => item.toUpperCase()
);

// arr2 = ['A', 'B', 'C']
```

___
[[10.01 Array Methods]]