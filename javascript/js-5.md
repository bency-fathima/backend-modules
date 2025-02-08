# Operators and Expressions in Programming

Operators are special symbols that perform specific operations on one or more operands. Expressions are combinations of values, variables, and operators that result in a new value.

## 1. Arithmetic Operators

Arithmetic operators perform mathematical calculations like addition, subtraction, multiplication, etc.

| Operator | Description        | Example        | Output |
|----------|------------------|---------------|--------|
| `+`      | Addition          | `5 + 3`       | `8`    |
| `-`      | Subtraction       | `5 - 3`       | `2`    |
| `*`      | Multiplication    | `5 * 3`       | `15`   |
| `/`      | Division          | `5 / 2`       | `2.5`  |
| `//`     | Floor Division    | `5 // 2`      | `2`    |
| `%`      | Modulus (Remainder) | `5 % 2`    | `1`    |
| `**`     | Exponentiation    | `5 ** 2`      | `25`   |

### Example:
```python
x = 10
y = 3
print(x + y)  # Output: 13
print(x - y)  # Output: 7
print(x * y)  # Output: 30
print(x / y)  # Output: 3.3333
print(x // y) # Output: 3
print(x % y)  # Output: 1
print(x ** y) # Output: 1000
```

## 2. Comparison (Relational) Operators

Comparison operators compare two values and return `True` or `False`.

| Operator | Description            | Example  | Output  |
|----------|------------------------|---------|---------|
| `==`     | Equal to                | `5 == 5` | `True`  |
| `!=`     | Not equal to            | `5 != 3` | `True`  |
| `>`      | Greater than            | `5 > 3`  | `True`  |
| `<`      | Less than               | `5 < 3`  | `False` |
| `>=`     | Greater than or equal to | `5 >= 3` | `True`  |
| `<=`     | Less than or equal to   | `5 <= 3` | `False` |

### Example:
```python
a = 10
b = 5
print(a == b)  # False
print(a != b)  # True
print(a > b)   # True
print(a < b)   # False
print(a >= b)  # True
print(a <= b)  # False
```

## 3. Logical Operators

Logical operators combine multiple conditions and return `True` or `False`.

| Operator | Description            | Example           | Output  |
|----------|------------------------|------------------|---------|
| `and`    | Returns `True` if both conditions are `True` | `True and False` | `False` |
| `or`     | Returns `True` if at least one condition is `True` | `True or False`  | `True`  |
| `not`    | Reverses the result    | `not True`        | `False` |

### Example:
```python
x = True
y = False
print(x and y)  # Output: False
print(x or y)   # Output: True
print(not x)    # Output: False
```

## Summary
- **Arithmetic operators** perform basic mathematical operations.
- **Comparison operators** compare values and return `True` or `False`.
- **Logical operators** are used to combine multiple conditions.

Using these operators, you can build complex expressions and logic in your programs.
