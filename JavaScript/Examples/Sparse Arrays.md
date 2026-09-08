#### Definition

**Sparse Array**
Arrays can contain empty slots, which are not the same as slots filled with the value undefined.

___
#### Examples

**Array Constructor**
```js
const a = Array(5); 
// [ <5 empty items> ]
```

**Array Literal**
```js
const b = [1, 2, , , 5]; 
// [ 1, 2, <2 empty items>, 5 ]
```

**Setting Length**
```js
const d = [1, 2]; d.length = 5; 
// [ 1, 2, <3 empty items> ]
```

**Deleting Element**
```js
const e = [1, 2, 3, 4, 5]; 
delete e[2]; 

// [ 1, 2, <1 empty item>, 4, 5 ]
```

___
[[10.03 Sparse Arrays]]