#### Definition

**props**
Props (short for properties) are values that a parent component passes to a child component.

___
#### Examples

**Passing Event Handler Prop**
Parent often owns the behavior that needs to change. Children can also do it but it will reduce the reusability of the child component. 
```tsx
function Parent() {
  const handleLongPress = () => {
    console.log('Long pressed');
  };

  return (
    <Child onLongPress={handleLongPress} />
  );
}

type ChildProps = {
  onLongPress: () => void;
};

function Child({ onLongPress }: ChildProps) {
  return (
    <Pressable onLongPress={onLongPress}>
      <Text>Click and Hold</Text>
    </Pressable>
  );
}
```

___
[[01.xx Component Composition]]