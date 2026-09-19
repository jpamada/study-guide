#### Definition

**relations()**
Defines relationships between Drizzle tables at the ORM level.

___
#### Import 

**drizzle-orm**
```ts
import { 
	relations 
} from "drizzle-orm";
```
___
#### Syntax

**one()**
```ts
export const tableOneRelations = relations(
  tableOne,
  ({ one }) => ({
    author: one(tableTwo, {
      fields: [tableOne.tableTwoId],
      references: [tableTwo.id],
    }),
  }),
);
```

**many()**
```ts
export const tableOneRelations = relations(
  tableOne,
  ({ many }) => ({
    posts: many(tableTwo),
  }),
);
```

___
[[01.04 Relations]]