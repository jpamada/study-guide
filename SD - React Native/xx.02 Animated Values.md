#### Definition

**Animated Value**
The initial value of the animated variable.

___
#### Examples

**[[Animated.Value()]]**
The value that drives an animation. The value changes over time while the animation is running.

**[[useAnimatedValue()]]**
The newer version and the wrapper of `Animated.Value.` already contains `useRef.`

___
#### Methods

**[[setValue()]]**
Immediately sets the value.

**[[stopAnimation()]]**
Stops the current animation and leaves the value where it stopped.

**[[resetAnimation()]]**
Stops the animation and resets the value to its original starting value.

___
#### Related Topic

**[[interpolate()]]**
Maps an animated value from one numeric range to another output range. Useful when the value corresponds to a string like background color.

___
[[xx.01 Animated|Prev]] | [[xx.03 Animated Components|Next]]