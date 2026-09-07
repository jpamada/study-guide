#### Definition

**Array.flatMap()**
Maps each element and then flattens the result by one level.

___
#### Syntax

**Syntax 1**
```js
array.flatMap(callback)
```

___
#### Examples

**Example 1**
```js
const arr1 = ["a", "b", "c"];

const arr2 = a1.flatMap(
	(item) => [
		item.toUpperCase(), 
		item.toLowerCase()
	]
);

// arr2 = [
//   'A', 'a', 'B', 'b', 'C', 'c'
// ];
```

___
[[09.01 Array Methods]]