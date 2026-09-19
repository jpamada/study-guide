#### Definition

**defineConfig()**
Helper function from drizzle-kit used to define and type-check the configuration for Drizzle Kit.

___
#### Import

**drizzle-kit**
```tsx
import { 
	defineConfig 
} from "drizzle-kit";
```

___
#### Syntax

**Basic Syntax**
```tsx
export default defineConfig({
  dialect: 'sqlite',
  schema: './src/db/schema'
})
```

___
#### Properties

**[[dialect]]**
Specifies the type of database you're working with.

**[[schema]]**
Specifies the path to your Drizzle schema file or folder.

**[[out]]**
Specifies where Drizzle Kit should put generated migration files and related metadata.

**[[driver]]**
Specifies a particular database driver when a database requires a special driver configuration.

___
[[01.02 Configuration]]