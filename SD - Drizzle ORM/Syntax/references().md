#### Definition

**dialect**
Specifies the type of database you're working with.

___
#### Syntax

**Basic Syntax**
```ts
columnType("column")
.references(() => tableTwo.column);
```

___
#### Example

**Basic Example**
```tsx
categoryId: text("category_id")
.references(() => categories.id),
```

___
[[sqliteTable()]]