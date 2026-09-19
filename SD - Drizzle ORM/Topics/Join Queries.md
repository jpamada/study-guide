#### Examples

**`leftJoin()`**  
Combines rows from two tables while keeping all rows from the left table.
```ts
db.select()
  .from(subjects)
  .leftJoin(
    categories,
    eq(subjects.categoryId, categories.id),
  );
```

**`rightJoin()`**  
Keeps all rows from the right table.
```ts
db.select()
  .from(subjects)
  .rightJoin(
    categories,
    eq(subjects.categoryId, categories.id),
  );
```

**`innerJoin()`**  
Returns rows where matching records exist in both tables.
```ts
db.select()
  .from(subjects)
  .innerJoin(
    categories,
    eq(subjects.categoryId, categories.id),
  );
```

**`fullJoin()`**  
Returns matching rows plus unmatched rows from both tables, where supported by the database/dialect.
```ts
db.select()
  .from(subjects)
  .fullJoin(
    categories,
    eq(subjects.categoryId, categories.id),
  );
```

___
[[Query Builder]]