#### Definition

**Animated.View**
Can handle the animated value and style the component.

___
#### Syntax

**Basic Syntax**
```tsx
<Animated.View
	style={{
		// style with animated variables
	}}
></Animated.View>
```

___
#### Examples

**Basic Example**
```tsx
const opacity = useAnimatedValue(0);

return (
	<Animated.View
		style={{ opacity }}
  >
  </Animated.View>
)
```

___
[[xx.03 Animated Components]]
