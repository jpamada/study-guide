#### Definition

**Transaction**
Groups multiple database operations into one logical unit so they can be committed together or rolled back together.

___
#### Syntax

**Basic Syntax**
```ts
await db.transaction(async (tx) => {
  // database operations
});
```

**With Promise**
Useful for executing multiple independent database operations within the same transaction. Not usefull if the second query needed the output of the first query.
```ts
await db.transaction(async (tx) => {
  await Promise.all([
    tx.insert(tableOne).values(...),
    tx.insert(tableTwo).values(...),
  ]);
});
```

___
#### Examples

**Basic Example**
If the second operation fails, the transaction can roll back the first operation.
```ts
await db.transaction(async (tx) => {
  await tx.insert(tableOne).values({
    id: "001",
  });

  await tx.insert(tableTwo).values({
    id: "002",
    folderId: "001",
  });
});
```

___
[[Advance Query]]