#### Definition

**Relational Query**
Designed around the relationships rather than explicitly constructing SQL clauses.

___
#### Results

**findMany()**
Fetches more than one row.
```ts
const tableName = await db.query.tableName
.findMany({
	// Query
});
```

**findFirst()**
Fetches the first row it find.
```ts
const tableName = await db.query.tableName
.findFirst({
	// Query
});
```

___
#### Something

**where**
```ts
const tableName = await db.query.tableName
.findMany({
  where: eq(
	  tableName.id, "123"
	),
});
```

**columns**
Select the included columns.
```ts
const tableName = await db.query.tableName
.findMany({
  columns: {
	  column1: true,
	  column2: true
  }
});
```

**with**
Uses the created relations. Can have nested with.
```ts
const tableOne = await db.query.tableOne
.findMany({
  with: {
	  tableTwo: true
  }
});
```

___
[[01.05 Queries]]