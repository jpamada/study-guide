#### Syntax

**Basic Syntax**
```ts
const animatedStyle = useAnimatedStyle(() => {
  return {
    // animated styles
  };
});
```

___
#### Examples

**Basic Example**
```ts
const translateX = useSharedValue(0);
const translateY = useSharedValue(0);

const animatedStyle = useAnimatedStyle(() => {
  return {
    transform: [
      {
        translateX: translateX.value,
        translateY: translateY.value
      },
    ],
  };
});
```