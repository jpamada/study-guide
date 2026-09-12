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
```jsx
const memoizedValue = useMemo(() => {
  return calculation;
}, [dependencies]);
```

**Basic Syntax (Shorter)**
```jsx
const memoizedValue = useMemo(
  () => calculation,
  [dependencies]
);
```

___
[[Hooks]]