#### Definition

**renderItem**
A function that receives each item from data and returns the React element that should be rendered. This prop is required.

___
#### Syntax

**Syntax 1**
```tsx
renderItem={({ item, index, separators }) => {
  return <Component />;
}}
```

___
#### Examples

**Example 1**
```tsx
<FlatList
  data={users}
  renderItem={({ item }) => (
    <Text>{item.name}</Text>
  )}
/>
```

___
#### Parameters

**item**
Current data item.

**index**
Current index.

**seperators**
Controls the item's separators.

___
[[FlatList]]