#### Examples

**`insert()`**  
Creates one or more new rows in a table.
```ts
await db
  .insert(subjects)
  .values({
    id: "1",
    name: "JavaScript",
  });
```

**`values()`**  
Specifies the values to insert.
```ts
.values({
  id: "1",
  name: "JavaScript",
});
```

___
[[Query Builder]]