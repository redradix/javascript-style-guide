# Redradix JavaScript Style Guide

<p align="center">
  <img src="https://raw.githubusercontent.com/redradix/javascript-style-guide/master/redradix-heart-js.png" width="300" alt="Redradix loves JavaScript"/>
</p>

## Table of Contents

1. [Naming 101](#naming-101)
1. [Strings](#strings)
1. [References](#references)


## Naming 101

- Use snake_case when naming files.
```
js_style_guide.js
```

- Use camelCase when naming objects, primitives, functions, and instances.
```javascript
var myObject = {};
var myNumber = 1;
var myFunc = function() {};
var myFuncInstance = new myFunc();
```

- Use PascalCase when naming singletones, constructors or classes.
```javascript
var MyClass = function() {};

class MyClass {}
```

- Use UPPERCASE when naming constants.
```javascript
const MY_CONSTANT = 1;
```

## Strings

- Use single quotes `''` for strings.
```javascript
var name = 'John Doe';
```

- Strings longer than 80 characters should be written across multiple lines using string concatenation.

- When programmatically building up strings, use template strings instead of concatenation.
```javascript
function sayHi(name) {
  return `How are you, ${name}?`;
}
```

##References

- Use `const` for all of your references; avoid using `var`.
```javascript
const a = 1;
```

- If you must mutate references, use `let`.
```javascript
let a = 1;
```

- Note that both `let` and `const` are block-scoped.
```javascript
// const and let only exist in the blocks they are defined in.
{
  let a = 1;
  const b = 1;
}
console.log(a); // ReferenceError
console.log(b); // ReferenceError
```