#### Definition

**integer()**
For integers, date and boolean.

___
#### Syntax

**Basic Syntax**
```ts
column: integer("column")
```

**Boolean**
```ts
column: integer("column", {
  mode: "boolean",
});
```

**Timestamp**
```tsx
column: integer("column", {
  mode: "timestamp",
});
```

**Timestamp Milliseconds**
```ts
column: integer("column", {
  mode: "timestamp_ms",
}),
```

___
[[sqliteTable()]]