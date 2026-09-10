#### Definition

**Object.groupBy()**
Can be used to group the elements of an array.

___
#### Syntax

**Syntax 1**
```js
Object.groupBy(items, callback)
```

**Callback Syntax**
```js
Object.groupBy(items, 
	(element, index) => {
	  return groupKey;
	}
);
```

___
#### Examples

**Example 1**
In this example the type is dereferenced.
```js
const inventory = [
  { 
	  name: "asparagus", 
	  type: "vegetables" 
	},
  { 
	  name: "bananas", 
	  type: "fruit" 
	},
  { 
	  name: "goat", 
	  type: "meat" 
	},
  { 
	  name: "cherries", 
	  type: "fruit" 
	},
  { 
	  name: "fish", 
	  type: "meat" 
	},
];

const result = Object.groupBy(
	inventory, ({ type }) => type
);

/*
{ 
vegetables: [
	{
		name: "asparagus",
		type: "vegetables"
	},
],
fruit: [
	{ 
		name: "bananas", 
		type: "fruit" 
	},
	{ 
		name: "cherries", 
		type: "fruit"
	} 
],
meat: [
	{
		name: "goat", 
		type: "meat" 
	}, 
	{ 
		name: "fish", 
		type: "meat" 
	}
]
}
*/
```

___
[[10.02 Array Transformation]]