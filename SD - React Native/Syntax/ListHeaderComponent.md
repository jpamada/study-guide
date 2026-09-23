#### Definition

**ListHeaderComponent**
Renders content above the list items.

___
#### Syntax

**Syntax 1**
```tsx
<FlatList ListHeaderComponent={Component} />
```

___
#### Examples

**Example 1**
```tsx
<FlatList
	ListHeaderComponent={
    <Text className="text-xl font-bold">
      Notes
    </Text>
  }
  data={notes}
  renderItem={({ item }) => (
    <NoteItem question={item} />
  )}
/>
```

___
[[FlatList]]