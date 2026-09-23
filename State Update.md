#### Definition

**State Update**
Updating state causes the screen render again. It doesn't need to throw away the entire screen.

___
#### Details 

**Normal Variables**
Changing the value of normal variables does not re-render the screen.

**useRef**
Changing the value of `useRef` does not also cause re-render.

___
[[02.01 Rendering]]