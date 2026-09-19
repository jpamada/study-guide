#### Examples

**`orderBy()`**  
Controls the order in which rows are returned.
```ts
db.select()
  .from(subjects)
  .orderBy(asc(subjects.name));
```

**`asc()`**  
Sorts values in ascending order.
```ts
asc(subjects.name)
```

**`desc()`**  
Sorts values in descending order.
```ts
desc(subjects.createdAt)
```

Multiple sorting columns:
```ts
.orderBy(
  asc(subjects.name),
  desc(subjects.createdAt),
)
```

___
[[Query Builder]]