#### Definition

**useContext**
Share data between components without passing props manually. Prevents prop drilling.

___
#### Syntax

**Basic Context**
```jsx
export const MyContext = 
	createContext(defaultValue);
```

```jsx
<MyContext value={value}>
  <App />
</MyContext>
```

```jsx
import {
  createContext
} from "react";

const value = useContext(MyContext);
```

**Provider**
```jsx
function MyProvider({ children }) {
  return (
    <MyContext value={value}>
      {children}
    </MyContext>
  );
}
```

```jsx
<MyProvider>
  <App />
</MyProvider>
```

**Provider + Custom Hook**
```jsx
const MyContext = createContext(null);

export function MyProvider({ 
	children 
}) {
  return (
    <MyContext value={value}>
      {children}
    </MyContext>
  );
}

export function useMyContext() {
  return useContext(MyContext);
}
```

```jsx
  <MyProvider>
    <App />
  </MyProvider>
```

```jsx
export default function App() {
  const { value } = 
	  useMyContext();
}
```

**Provider + Custom Hook + Error Check**
```jsx
export function useMyContext() {
  const context = 
	  useContext(MyContext);

  if (!context) {
    throw new Error("Error Message");
  }

  return context;
}
```

___
[[Context Hooks]]