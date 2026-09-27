#### Definition

**Debouncing**
Delays executing a function until a certain amount of time has passed without another call occurring.

___
#### Examples
This example debounces `500ms.`
```jsx
import { useEffect, useState } from 'react';

function SearchInput() {
  const [search, setSearch] = useState('');

  useEffect(() => {
    const timeout = setTimeout(() => {
      console.log('Searching:', search);
    }, 500);

    return () => {
      clearTimeout(timeout);
    };
  }, [search]);

  return (
    <input
      value={search}
      onChange={(event) => setSearch(event.target.value)}
      placeholder="Search..."
    />
  );
}
```

