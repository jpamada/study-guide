#### Definition

**Upsert Queries**
Insert the record if it doesn't exist and update it if a conflict occurs.

___
#### Syntax

**Basic Syntax**
```ts
await db
  .insert(table)
  .values({
    id: "1",
    name: "Name",
  })
  .onConflictDoUpdate({
    target: table.id,
    set: {
      name: "Name Updated",
    },
  });
```

___
[[Advance Query]]