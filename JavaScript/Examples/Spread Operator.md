#### Examples

**Example 1**
Spread with objects.
```js
const user = {
  name: "John",
  age: 25,
};

const updatedUser = {
  ...user,
  age: 26,
};
```

**Example 2**
Spread with array.
```js
const users = ["John", "Jane"];

const newUsers = [
  ...users, 
  "Bob"
];
```

___
[[05.03 Spread Operator]]