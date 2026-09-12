#### Definition

**useRef**
Store a value that persists between renders without causing a re-render when it changes.

___
#### Syntax

**Basic**
```jsx
const valueRef = useRef(initialValue);

valueRef.current;

valueRef.current = newValue;
```

**Accessing DOM Element**
```jsx
const inputRef = useRef(null);

inputRef.current

<input ref={inputRef} />
```

****
#### Examples

**Basic**
```jsx
const countRef = useRef(0);

function increaseCount() {
	countRef.current += 1;
}

<button onClick={increaseCount}>
	Increase
</button>
```

**Accessing DOM Element**
```jsx
const inputRef = useRef(null);

function focusInput() {
	inputRef.current.focus();
}

<input ref={inputRef} />

<button onClick={focusInput}>
	Focus Input
</button>
```

___
[[Hooks]]