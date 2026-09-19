#### Definition

**Animated.timing()**
Animates a value over time using an easing curve.

___
#### Syntax

**Basic Syntax**
```ts
Animated.timing(value, config);
```

**With Method**
```ts
Animated.timing(value, config).start();
```

___
#### Config Options

**duration**
Length of animation, in milliseconds.

**easing**
Easing function defining the curve.

**delay**
Delay (ms) before the animation starts.

**isInteraction**
Whether this animation creates an "interaction handle."

**useNativeDriver**
Whether to run on the native thread. This is required.

___
[[xx.04 Animated Types]]