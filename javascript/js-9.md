# JavaScript for Loop

## Introduction
The `for` loop in JavaScript is used for executing a block of code repeatedly until a specified condition is met. It is commonly used for iterating over arrays, performing calculations, and running repeated tasks.

### Syntax
```javascript
for (initialization; condition; increment/decrement) {
    // Code to execute in each iteration
}
```

### Explanation
1. **Initialization**: This is executed once before the loop starts. It usually initializes a loop variable.
2. **Condition**: The loop runs as long as this condition evaluates to `true`.
3. **Increment/Decrement**: Updates the loop variable after each iteration.
4. **Loop Body**: The block of code to be executed in each iteration.

### Example
```javascript
for (let i = 1; i <= 5; i++) {
    console.log("Iteration number: " + i);
}
```

### Output
```
Iteration number: 1
Iteration number: 2
Iteration number: 3
Iteration number: 4
Iteration number: 5
```

## Nested for Loop
A `for` loop can be nested inside another `for` loop.

### Example
```javascript
for (let i = 1; i <= 3; i++) {
    for (let j = 1; j <= 2; j++) {
        console.log(`i = ${i}, j = ${j}`);
    }
}
```

### Output
```
i = 1, j = 1
i = 1, j = 2
i = 2, j = 1
i = 2, j = 2
i = 3, j = 1
i = 3, j = 2
```

## When to Use for Loop?
- When the number of iterations is known beforehand.
- To iterate over arrays or collections efficiently.
- When a loop requires an initializer, condition, and an increment/decrement step.

## Conclusion
The `for` loop is one of the most widely used looping constructs in JavaScript, offering efficiency and control over repeated execution.
