#### Definition

**Array.splice()**
Removes elements from an array and (optionally) replaces them. It returns the items which were removed from the array.

___
#### Syntax

**Syntax 1**
```js
array.splice(
	start, 
	deleteCount, 
	item1, 
	item2, 
	...
);
```

___
#### Examples

**Example 1**
```js
const arr = ["1", "2", "3", "4"]; 

arr.splice(1, 2, "a", "b");

// arr = ["1", "a", "b", "4"]
```

___
[[09.01 Array Methods]]