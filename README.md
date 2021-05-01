# Javascript Annotations

### Spread Syntax (...)

It can be applied over arrays, objects and even strings.

Example:
```typescript
const arr: number[] = [12, 23, 34, 45, 56, 67, 78, 89, 90];
const newArr = [...arr]; // This will create a new copy of the previous array.
const thirdArr = newArr;
console.log(thirdArr === newArr);
```
