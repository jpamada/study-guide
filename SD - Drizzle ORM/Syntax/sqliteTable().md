#### Definition

**sqliteTable()**
Drizzle ORM function that define a SQLite database table.

___
#### Syntax

**Basic Syntax**
```ts
export const tableName = sqliteTable("table_name", {
  columnName: columnType(
	  "column_name"
  ),
});
```

**With Table Configuration**
```ts
export const table = sqliteTable(
"table_name",
{
	columnName: columnType(
		"column_name"
	),
},
(table) => [
	foreignKey({
		columns: [table.categoryId],
		foreignColumns: [categories.id],
	}),
]);
```

___
#### Example

**Basic Syntax**
```ts
export const users = sqliteTable("users", {
  id: text("id").primaryKey(),
  
  name: text("name").notNull(),
  
  age: integer("age"),
  
  createdAt: integer("created_at", { 
	  mode: "timestamp_ms" 
	}).notNull(),
});
```

#### Column Types

**[[text()]]**
For string data.

**[[integer()]]**
For integers, date and boolean.

___
#### Column Constraints

**[[primaryKey()]]**
Makes the column the primary key.

**[[notNull()]]**
Prevents `null.`

**[[default()]]**
Provides a default value.

**[[references()]]**
Creates a foreign-key reference.

#### Configuration

**[[Table Configuration]]**

___
[[01.03 Schema]]