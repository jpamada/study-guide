#### Syntax

**Old Syntax**
```ts
const pan = Gesture.Pan()
  .onUpdate((event) => {
    // event
  });
```

**New Syntax**
```ts
const pan = usePanGesture({
	onUpdate: (event) => {
		// event
	};
})
  
```