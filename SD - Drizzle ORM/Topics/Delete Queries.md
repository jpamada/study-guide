#### Examples

**delete()**  
Deletes rows from a table.
```ts
await db
  .delete(subjects)
  .where(eq(subjects.id, "1"));
```

___
[[Query Builder]]