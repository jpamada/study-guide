#### Examples

**`sql`**  
Allows you to write a SQL expression when Drizzle's normal query builders aren't sufficient.
```ts
db.select({
  name: subjects.name,
  customValue: sql`...`,
})
.from(subjects);
```

___
[[Query Builder]]