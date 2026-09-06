**Example 1**
Creates shadowing that declares inner variable the same name as outer variable.
```js
let name = "John";

{
	let name = "Jane";
	console.log(name); // Jane
}

console.log(name); // John
```

**Example 2**
`var` declared variables are not block-scoped.
```js
var x = 1;

{
  var x = 2;
}

console.log(x); // 2
```

___
[[01.01 Variable Scopes]]