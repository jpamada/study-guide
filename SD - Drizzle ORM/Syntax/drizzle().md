#### Definition

**drizzle()**
Drizzle ORM function that creates a Drizzle database instance from a database connection.

___
#### Import

**drizzle-orm**
```tsx
import { 
	drizzle 
} from "drizzle-orm/expo-sqlite";
```

___
#### Syntax

**Basic Syntax**
```tsx
const sqliteDb = openDatabaseSync(
	"dbName.db"
);
const db = drizzle(sqliteDb);
```

___
#### Example

**Basic Example**
```tsx
const db = drizzle(sqliteDatabase);
```

**With Schema**
```ts
import * as 
	schema 
from './schema';

export const db = drizzle(expoDb, {
  schema,
});
```

**With Schema and Relation**
```ts
import * as 
	schema 
from './schema';

import * as 
	relations 
from './relations';

export const db = drizzle(expoDb, {
  schema: {
    ...schema,
    ...relations,
  },
});
```


___
[[01.01 Connection]]