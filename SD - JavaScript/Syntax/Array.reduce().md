#### Definition

**Array.reduce()**
Combines all array elements into a single value.

___
#### Syntax

**Syntax 1**
```js
array.reduce(
	(
		accumulator, 
		element, 
		index, 
		array
	) => {
  return newValue;
}, initialValue)
```

___
#### Examples

**Example 1**
```js
const arr = [10, 20, 30];

const total = arr.reduce(
  (accumulator, currentValue) => {
	  accumulator + currentValue, 0
  }  
);

// total = 60
```

___
[[10.01 Array Methods]]