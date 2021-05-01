# Javascript Annotations

### Spread Syntax (...)

Allows an iterable such as an array expression or string to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected, or an object expression to be expanded in places where zero or more key-value pairs (for object literals) are expected.

It helps us (when it comes to arrays and objects) to avoid mutating objects and creating new instances instead of using values as references.

*Example (Arrays):*
```javascript
const arr = [12, 23, 34, 45, 56, 67, 78, 89, 90];
const newArr = [...arr]; // This will create a new copy of the previous array.
const thirdArr = newArr;
console.log(thirdArr === newArr); // Will be true
```

*Example (Objects):*
```javascript
const customObj = {
  name: 'John', 
  lastName: 'Doe'
}

// Don't
const newObj = customObj;
newObj.age = 23;

// Do
const anotherObj = {
  ...customObj, 
  age: 26
};

console.log(customObj) // Will be mutated and include age 23.

```

*Example (String):*
```javascript
const testStr = 'hello world';
const arrConverted = [...testStr];
console.log(arrConverted); // Will return ['h','e','l','l,''o,' ','w','o','r','l','d'];
```
