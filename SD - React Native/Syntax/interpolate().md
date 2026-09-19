#### Definition

**interpolate()**
Maps an animated value from one numeric range to another output range.

___
#### Syntax

**Basic Syntax**
This basical maps the `inputRange: [0, 1]` as `[0, 100].` Meaning if the animated value is 0 it is zero and if it's 1 then it is 100.
```ts
const value = new Animated.Value(0);

const output = value.interpolate({
  inputRange: [0, 1],
  outputRange: [0, 100],
});
```

___
[[xx.02 Animated Values]]