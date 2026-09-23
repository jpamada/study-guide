#### Definition

**ItemSeparatorComponent**
It does not render at the beginning or end of the list.

___
#### Syntax

**Syntax 1**
```tsx
<FlatList ItemSeparatorComponent={Component} />
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
  ItemSeparatorComponent={() => (
    <View className="h-px bg-gray-300" />
  )}
/>
```

___
[[FlatList]]
