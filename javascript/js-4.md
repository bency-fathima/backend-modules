# Basic Syntax and Data Types in JavaScript

## 1. Variables and Their Scope

In JavaScript, variables can be declared using `let`, `const`, and `var` (though `var` is rarely used in modern JavaScript).

### `let` and `const`
- `let`: Used for variables that can be reassigned.
- `const`: Used for variables that cannot be reassigned.

#### Example:
```js
let name = "John"; // Can be reassigned
const age = 30; // Cannot be reassigned
```

### Scope of Variables
- **Global Scope**: A variable declared outside any function is globally scoped.
- **Block Scope**: `let` and `const` have block scope, meaning they exist only within the `{}` they are declared in.
- **Function Scope**: Variables declared inside a function exist only within that function.

#### Example:
```js
function testScope() {
    let localVar = "I'm inside the function";
    console.log(localVar); // Accessible here
}
// console.log(localVar); // Error: localVar is not defined
```

## 2. JavaScript Data Types
JavaScript has several primitive data types:

### 1. **String**
Used for text values.
```js
let message = "Hello, World!";
```

### 2. **Number**
Represents both integers and floating-point numbers.
```js
let count = 42;
let price = 99.99;
```

### 3. **Boolean**
Represents `true` or `false` values.
```js
let isActive = true;
```

### 4. **Null**
Represents an intentional absence of any value.
```js
let emptyValue = null;
```

### 5. **Undefined**
Represents an uninitialized variable.
```js
let notAssigned;
console.log(notAssigned); // undefined
```

### 6. **Symbol** (Introduced in ES6)
Represents unique values that are immutable.
```js
let sym1 = Symbol("identifier");
let sym2 = Symbol("identifier");
console.log(sym1 === sym2); // false
```

## Summary
| Data Type  | Description |
|------------|-------------|
| String | Represents text values |
| Number | Represents both integers and floats |
| Boolean | Represents `true` or `false` |
| Null | Represents the absence of value |
| Undefined | Represents an uninitialized variable |
| Symbol | Unique and immutable identifier |

Understanding these basic concepts is crucial for mastering JavaScript programming.
