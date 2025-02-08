# Operators and Expressions in Programming

## 1. Arithmetic Operators
Arithmetic operators are used to perform mathematical operations such as addition, subtraction, multiplication, etc.

| Operator | Description          | Example    | Output |
|----------|----------------------|------------|--------|
| `+`      | Addition             | `5 + 3`    | `8`    |
| `-`      | Subtraction          | `5 - 3`    | `2`    |
| `*`      | Multiplication       | `5 * 3`    | `15`   |
| `/`      | Division             | `5 / 2`    | `2.5`  |
| `%`      | Modulus (Remainder)  | `5 % 2`    | `1`    |
| `**`     | Exponentiation       | `5 ** 2`   | `25`   |
| `//`     | Floor Division       | `5 // 2`   | `2`    |

### Example:
```python
x = 10
y = 3
print(x + y)  # Output: 13
print(x - y)  # Output: 7
print(x * y)  # Output: 30
print(x / y)  # Output: 3.3333
print(x % y)  # Output: 1
print(x ** y) # Output: 1000
print(x // y) # Output: 3
```

---

## 2. Comparison Operators
Comparison operators are used to compare values.

| Operator | Description                | Example     | Output  |
|----------|----------------------------|-------------|---------|
| `==`     | Equal to                    | `5 == 3`    | `False` |
| `!=`     | Not equal to                | `5 != 3`    | `True`  |
| `>`      | Greater than                | `5 > 3`     | `True`  |
| `<`      | Less than                   | `5 < 3`     | `False` |
| `>=`     | Greater than or equal to    | `5 >= 3`    | `True`  |
| `<=`     | Less than or equal to       | `5 <= 3`    | `False` |

### Example:
```python
x = 5
y = 3
print(x == y)  # Output: False
print(x != y)  # Output: True
print(x > y)   # Output: True
print(x < y)   # Output: False
print(x >= y)  # Output: True
print(x <= y)  # Output: False
```

---

## 3. Logical Operators
Logical operators are used to combine conditional statements.

| Operator | Description           | Example        | Output  |
|----------|-----------------------|---------------|---------|
| `and`    | Returns `True` if both conditions are true | `True and False` | `False` |
| `or`     | Returns `True` if at least one condition is true | `True or False` | `True`  |
| `not`    | Reverses the Boolean value | `not True` | `False` |

### Example:
```python
x = True
y = False
print(x and y)  # Output: False
print(x or y)   # Output: True
print(not x)    # Output: False
```

---

## 4. Control Structures
Control structures help manage the flow of execution in a program.

### 4.1 If/Else Statements
Used to execute different blocks of code based on conditions.

#### Example:
```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```

---

### 4.2 Loops
Loops are used to execute a block of code multiple times.

#### 4.2.1 For Loop
```python
for i in range(5):
    print(i)  # Output: 0, 1, 2, 3, 4
```

#### 4.2.2 While Loop
```python
x = 0
while x < 5:
    print(x)
    x += 1
```

---

### 4.3 Iterating Over Collections

#### 4.3.1 The `for...of` Loop (JavaScript) - Used for iterating over arrays
```javascript
const numbers = [1, 2, 3, 4, 5];
for (const num of numbers) {
    console.log(num);  // Output: 1, 2, 3, 4, 5
}
```

#### 4.3.2 The `for...in` Loop (JavaScript) - Used for iterating over object properties
```javascript
const person = { name: "Alice", age: 25, city: "New York" };
for (const key in person) {
    console.log(`${key}: ${person[key]}`);
}
```

---

## Conclusion
Operators and control structures are fundamental concepts in programming. Understanding them is essential for writing efficient and functional programs.
