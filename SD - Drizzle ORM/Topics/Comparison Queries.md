#### Examples

**`eq()`**  
Checks whether two values are equal (`=`).
```ts
eq(subjects.id, "1")
```

**`ne()`**  
Checks whether two values are not equal (`<>`).
```ts
ne(subjects.id, "1")
```

**`isNull()`**  
Checks whether a column is `NULL`.
```ts
isNull(subjects.categoryId)
```

**`isNotNull()`**  
Checks whether a column is not `NULL`.
```ts
isNotNull(subjects.categoryId)
```

**`gt()`** 
Checks whether a value is greater than another (`>`).
```ts
gt(subjects.position, 5)
```

**`gte()`**  
Checks whether a value is greater than or equal to another (`>=`).
```ts
gte(subjects.position, 5)
```

**`lt()`**  
Checks whether a value is less than another (`<`).
```ts
lt(subjects.position, 5)
```

**`lte()`**  
Checks whether a value is less than or equal to another (`<=`).
```ts
lte(subjects.position, 5)
```

___
[[Query Builder]]