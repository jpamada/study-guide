#### Definition

**Animated.Value**
The value that drives an animation. The value changes over time while the animation is running.

___
#### Syntax

**Basic Syntax**
```ts
const value = new Animated.Value(0);
```

**With useRef**
The common way of creating `Animated.Value.`
```ts
const value = useRef(new Animated.Value(0)).current;
```

___
[[04.02 Animated Values]]