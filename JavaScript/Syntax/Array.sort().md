#### Definition

**Array.sort()**
Sorts the elements of an array.

___
#### Syntax

**Syntax 1**
```js
array.sort()
```

**Syntax 2**
```js
array.sort(compareFunction)
```

___
#### Examples

**Example 1**
```js
const arr = [
	"Wind", "Rain", "Fire"
];

arr.sort();

// arr = ["Fire", "Rain", "Wind"]
```

**Sorting with Numbers**
```js
const nums = [10, 2, 30, 5];

nums.sort((a, b) => a - b);

// nums = [2, 5, 10, 30]
```

___
[[09.01 Array Methods]]