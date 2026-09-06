#### Examples

**Example 1**
Valid because `const` does NOT prevent mutation.
```javascript
const obj = { 
	key: "value" 
};

obj.key = "otherValue";
```

**Example 2**
Valid because the contents of an array are not protected.
```js
const arr = ["HTML", "CSS"];

arr.push("JS");
```

___
[[01.03 Constants]]