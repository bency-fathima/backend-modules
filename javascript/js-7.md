# JavaScript if-else Statement

## Introduction
The `if-else` statement in JavaScript is used for decision-making. It allows the program to execute certain blocks of code based on specified conditions.

### Syntax
```javascript
if (condition) {
    // Code to execute if condition is true
} else {
    // Code to execute if condition is false
}
```

### Explanation
1. The `if` statement evaluates the condition inside the parentheses `()`. 
2. If the condition is `true`, the code inside the `{}` block following `if` executes.
3. If the condition is `false`, the code inside the `else` block executes.

### Example
```javascript
let age = 18;

if (age >= 18) {
    console.log("You are eligible to vote.");
} else {
    console.log("You are not eligible to vote.");
}
```

### Output
```
You are eligible to vote.
```

## Nested if-else
You can also use `if-else` inside another `if-else`, known as a nested `if-else`.

### Example
```javascript
let score = 85;

if (score >= 90) {
    console.log("Grade: A");
} else if (score >= 80) {
    console.log("Grade: B");
} else {
    console.log("Grade: C or below");
}
```

### Output
```
Grade: B
```

## Conclusion
The `if-else` statement is fundamental for control flow in JavaScript, enabling conditional execution of code based on logic and expressions.
