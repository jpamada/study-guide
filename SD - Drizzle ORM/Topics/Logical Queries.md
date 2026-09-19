#### Examples

**`and()`**  
Combines conditions where **all conditions must be true**.
```ts
where(
  and(
    eq(subjects.categoryId, "1"),
    eq(subjects.deletedAt, null),
  ),
)
```

**`or()`**  
Combines conditions where **at least one condition must be true**.
```ts
where(
  or(
    eq(subjects.name, "JavaScript"),
    eq(subjects.name, "TypeScript"),
  ),
)
```

**`not()`**  
Negates a condition.
```ts
where(
  not(eq(subjects.name, "JavaScript")),
)
```

___
[[Query Builder]]