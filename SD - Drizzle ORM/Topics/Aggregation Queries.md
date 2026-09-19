#### Examples

**`count()`**  
Counts rows or values.
```ts
db.select({
  count: count(),
})
.from(subjects);
```

**`sum()`**  
Calculates the sum of a numeric column.
```ts
sum(subjects.position)
```

**`avg()`**  
Calculates the average of a numeric column.
```ts
avg(subjects.position)
```

**`min()`**  
Gets the minimum value.
```ts
min(subjects.position)
```

**`max()`**  
Gets the maximum value.
```ts
max(subjects.position)
```

___
[[Query Builder]]