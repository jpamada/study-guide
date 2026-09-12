#### Definition

**useEffect**
Connect a component to an exteral system.

___
#### Syntax

**Basic**
Code that runs after rendering
```jsx
useEffect(() => {
	// Code
});
```

**Empty Dependency Array**
Run when component mounts
```jsx
useEffect(() => {
  // Code
}, []);
```

**With Dependencies**
Run the effect again when one of the dependency changes.
```jsx
useEffect(() => {
  // Code
}, [dependency]);
```

**Cleanup Function**
```jsx
useEffect(() => {
  // Code

  return () => {
    // Cleanup
  };
}, []);
```

___
#### Examples

**Cleanup Function**
```jsx
  const [count, setCount] = useState(0);

  useEffect(() => {
    const timer = setInterval(() => {
			setCount(currentCount => {
				currentCount + 1;
			});
		}, 1000);

    return () => {
      clearInterval(timer);
    };
  }, []);
```

___
[[Hooks]]