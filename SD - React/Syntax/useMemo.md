#### Definition

**useMemo**
Cache the result of an expensive calculation.

___
#### Comparison

**[[useCallback]]**
Unlike calculation useCallback cache functions.

___
##### Syntax

**Basic Syntax**
Because a function body `{}` is added, return is required. Prefer it for readability.
```jsx
const memoizedValue = useMemo(() => {
  return calculation;
}, [dependencies]);
```

**Basic Syntax (Shorter)**
Automatically returns the calculation.
```jsx
const memoizedValue = useMemo(
  () => calculation,
  [dependencies]
);
```

___
[[Hooks]]