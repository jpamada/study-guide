#### Examples

**`distinct()`**  
Removes duplicate rows from the result.
```ts
db
  .selectDistinct({
    categoryId: subjects.categoryId,
  })
  .from(subjects);
```

___
[[Query Builder]]