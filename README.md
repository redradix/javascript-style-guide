# Redradix JavaScript Style Guide

<p align="center">
  <img src="https://raw.githubusercontent.com/redradix/javascript-style-guide/master/redradix-heart-js.png" width="300" alt="Redradix loves JavaScript"/>
</p>

## Table of Contents

1. [Naming 101](#naming-101)
1. [Strings](#strings)

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