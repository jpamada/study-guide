#### Examples

**`set()`**  
Specifies the columns and new values for an update.
```ts
.set({
  name: "Advanced JavaScript",
})
```

**`update()`**  
Specifies the table whose existing rows will be modified.
```ts
await db
  .update(subjects)
  .set({
    name: "Advanced JavaScript",
  })
  .where(eq(subjects.id, "1"));
```

___
[[Query Builder]]