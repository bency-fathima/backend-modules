# JavaScript switch Statement

## Introduction
The `switch` statement in JavaScript is used for decision-making and is an alternative to multiple `if-else` conditions. It evaluates an expression and executes code based on matching cases.

### Syntax
```javascript
switch(expression) {
    case value1:
        // Code to execute if expression matches value1
        break;
    case value2:
        // Code to execute if expression matches value2
        break;
    default:
        // Code to execute if no case matches
}
```

### Explanation
1. The `expression` inside `switch` is evaluated.
2. If the expression matches a `case` value, the corresponding block of code executes.
3. The `break` statement prevents fall-through to the next case.
4. The `default` block executes if no case matches.

### Example
```javascript
let day = 3;

switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    case 3:
        console.log("Wednesday");
        break;
    default:
        console.log("Invalid day");
}
```

### Output
```
Wednesday
```

## When to Use switch?
- Use `switch` when checking a variable against multiple values.
- It enhances readability and can be more efficient than multiple `if-else` statements.

## Conclusion
The `switch` statement is useful for handling multiple conditions efficiently and making the code more readable.
