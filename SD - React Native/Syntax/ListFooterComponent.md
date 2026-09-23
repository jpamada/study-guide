#### Definition

**ListFooterComponent**
Renders content after the list items.

___
#### Syntax

**Syntax 1**
```tsx
<FlatList ListFooterComponent={Component} />
```

___
#### Examples

**Example 1**
```tsx
<FlatList
  data={questions}
  renderItem={({ item }) => (
    <QuestionItem question={item} />
  )}
  ListFooterComponent={
    <Text>End of questions</Text>
  }
/>
```

___
[[FlatList]]
