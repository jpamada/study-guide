#### Examples

**Rest Parameter**
allow a function to accept multiple arguments.
```js
function test(...values) {
  console.log(values);
}
```

**Destructuring Object**
```js
const user = {
  name: "John",
  age: 25,
  role: "Admin",
};

const { name, ...rest } = user;

console.log(name); 
// "John"

console.log(rest);
// { age: 25, role: "Admin" }
```

___
[[04.05 Argument Object]] | [[05.03 Spread Operator]]