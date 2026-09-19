#### Examples

**[[select()]]**  
Retrieves data from one or more database tables.
```ts
const result = await db
.select()
.from(subjects);
```

**[[from()]]**  
Specifies the table to retrieve data from.
```ts
await db
.select()
.from(subjects);
```

**[[where()]]**  
Filters the rows returned or affected by a query.
```ts
db
.select()
.from(subjects)
.where(
	eq(subjects.id, "1")
);
```

___
[[Query Builder]]