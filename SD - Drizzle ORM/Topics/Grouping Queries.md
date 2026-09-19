#### Examples

**`groupBy()`**  
Groups rows based on one or more columns, commonly used with aggregate functions.
```ts
db.select({
  categoryId: subjects.categoryId,
  count: count(),
})
.from(subjects)
.groupBy(subjects.categoryId);
```

**`having()`**  
Filters grouped results after `groupBy()`.
```ts
db.select({
  categoryId: subjects.categoryId,
  count: count(),
})
.from(subjects)
.groupBy(subjects.categoryId)
.having(gt(count(), 5));
```

___
[[Query Builder]]