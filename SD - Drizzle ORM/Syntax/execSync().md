#### Definition

**execSync()**
Execute SQL synchronously.

___
#### Syntax

**Basic Syntax**
```ts
db.execSync(sql);
```

___
#### Example

**Basic Example**
```ts
db.execSync(`
  CREATE TABLE IF NOT EXISTS users(
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL
  );
`);
```

**Pragma Foreign Keys**
Enable foreign-key constraint enforcement in SQLite.
```ts
expoDb.execSync(
	'PRAGMA foreign_keys = ON;'
);
```

___
[[defineConfig()]]