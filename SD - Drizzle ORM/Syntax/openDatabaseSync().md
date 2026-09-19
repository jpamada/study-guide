#### Definition

**openDatabaseSync()**
Expo SQLite function that synchronously opens a SQLite database. It returns an Expo SQLite SQLiteDatabase instance that provides methods for executing SQL, transactions, prepared statements, etc.

___
#### Import

**expo-sqlite**
```tsx
import { 
	openDatabaseSync 
} from "expo-sqlite";
```

___
#### Syntax

**Basic Syntax**
```tsx
const db = openDatabaseSync(
	"database.db"
);
```

___
#### Examples

**Basic Example**
Opens or create `myDatabase`.
```tsx
const db = openDatabaseSync(
	"myDatabase.db"
);
```

___
#### Methods

**[[execSync()]]**
Execute SQL synchronously.

**[[execAsync()]]**
Execute SQL asynchronously.

___
[[01.01 Connection]]