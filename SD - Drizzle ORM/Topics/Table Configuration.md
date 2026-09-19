#### Syntax

**Index**
```tsx
export const table = sqliteTable(
"table",
{
	// columns
},
(table) => [
	index("subjects_name_idx").on(table.name),
]);
```

**Multiple Column Index**
```ts
(table) => [
  index("subjects_name_id_idx").on(
    table.name,
    table.id,
  ),
]
```

**Foreign Key**
```ts
(table) => [
  foreignKey({
    columns: [table.categoryId],
    foreignColumns: [categories.id],
    name: "subjects_category_id_fk",
  }),
]
```

**Foreign Key Behaviors**
```ts
(table) => [
  foreignKey({
    columns: [table.categoryId],
    foreignColumns: [categories.id],
  })
	.onDelete("set null")
	.onUpdate("cascade"),
]
```

**Unique**
```ts
(table) => [
  unique("users_email_unique").on(
	  table.email
	),
]
```

#### Foreign Key Actions

**"cascade"**
Deletes the child row.

**"restrict"**
Prevents deleting the parent.

**"no action"**
No automatic action; FK is still enforced.

**"set null"**
Sets the FK column to NULL.

**"set default"**
Sets the FK column to its default value.

___
[[sqliteTable()]]