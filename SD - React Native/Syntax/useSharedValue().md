#### Definition

**useSharedValue()**
Lets you define shared values in your components.

___
#### Syntax

**Basic Syntax**
```ts
const value = useSharedValue(0);
```

___
#### Example

**Basic Example**
```ts
const translateX = useSharedValue(0)

const moveBox = () => { 
	translateX.value = 100; 
};
```