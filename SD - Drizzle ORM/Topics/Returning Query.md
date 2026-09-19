#### Examples

**`returning()`**  
Returns the rows affected by an `insert`, `update`, or `delete` operation when supported by the dialect.
```ts
const result = await db
  .insert(subjects)
  .values({
    id: "1",
    name: "JavaScript",
  })
  .returning();
```

___
[[Query Builder]]