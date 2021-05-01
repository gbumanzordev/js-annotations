# Javascript Annotations

### Spread Syntax (...)

Allows an iterable such as an array expression or string to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected, or an object expression to be expanded in places where zero or more key-value pairs (for object literals) are expected.

Example (Arrays):
```typescript
const arr: number[] = [12, 23, 34, 45, 56, 67, 78, 89, 90];
const newArr = [...arr]; // This will create a new copy of the previous array.
const thirdArr = newArr;
console.log(thirdArr === newArr);
```

Example (Objects): 
```typescript
const customObj = {
  name: 'John', 
  lastName: 'Doe'
}
```
