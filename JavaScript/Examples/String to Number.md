#### Examples

**parseInt()**
Best practice is to use radix parameter.
```js
parseInt("101", 10); // 101
parseInt("101", 2);  // 5
parseInt("101", 8);  // 65
parseInt("101", 16); // 257
```

**parseFloat()**
All returns 3.14.
```js
parseFloat(3.14);
parseFloat("3.14");
parseFloat("  3.14  ");
parseFloat("314e-2");
parseFloat("0.0314E+2");
parseFloat("3.14some characters");
```

**Number()**
Returns `NaN` if parameter is non-numeric.
```js
Number("123");          // 123
Number("123") === 123;  // true
Number("unicorn");      // NaN
Number(undefined);      // NaN
```

**Binary Plus Operator**
String concatenation with binary plus operator.
```js
const z = "37" + 7; // 377
```

**Unary Operator**
```js
const z = +"37";

console.log(z);        // 37
console.log(typeof z); // Number
```

___
[[02.01 String to Number]]