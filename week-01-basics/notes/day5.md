# Day 5: Functions, Lambda, and Zip Functions

## 1. Functions in Python

Functions are reusable blocks of code designed to perform a specific task, helping to avoid code repetition (DRY - Don't Repeat Yourself).

### Key Concepts

- **Defining**: Declared using the `def` keyword followed by the function name and parentheses `()`.
- **Calling**: Executed by writing the function name with parentheses: `my_function()`.
- **Arguments & Parameters**:
  - **Parameters**: Variables listed in the function definition (e.g., `def greet(name):`).
  - **Arguments**: Actual values passed to the function when calling it (e.g., `greet("Alice")`).
- **Return Statement**: Uses the `return` keyword to send a result back to the caller. If no return is specified, the function returns `None`.

### Parameter Types

- **Default Parameters**: Standard values used if no argument is passed (e.g., `def power(base, exp=2):`).
- **Keyword Arguments**: Passing arguments using the parameter name so order doesn't matter (e.g., `greet(lastname="Doe", firstname="John")`).
- **Arbitrary Arguments (`*args`)**: Receives a tuple of arguments when the exact number is unknown.
- **Arbitrary Keyword Arguments (`**kwargs`)**: Receives a dictionary of keyword arguments.

## 2. Lambda Functions

Lambda functions are small, short-lived, anonymous (unnamed) functions defined in a single line.

### Key Rules

- **Syntax**: `lambda arguments: expression`
- **Single Expression**: They can take any number of arguments but can only contain one expression (which is automatically returned).
- **Usage**: Best used as short, temporary functions inside higher-order functions like `map()`, `filter()`, or `sorted()`.

### Example

```python
# Regular Function
def double(x):
    return x * 2

# Lambda equivalent
double_lambda = lambda x: x * 2
print(double_lambda(5))  # Output: 10
```

## 3. The `zip()` Function

The `zip()` function takes multiple iterables (like lists, tuples, or strings) and aggregates their corresponding elements into tuples.

### Key Features

- **Pairing**: It pairs the 1st elements together, then the 2nd elements, and so on.
- **Unequal Lengths**: If the input iterables have different lengths, `zip()` stops pairing at the shortest iterable (excess elements are ignored).
- **Unzipping**: You can unpack/unzip a zipped collection back into separate sequences using the zip operator with `*`: `zip(*zipped_object)`.

### Example

```python
names = ["Alice", "Bob", "Charlie"]
scores = [85, 90, 95]

# Pairing elements
paired = list(zip(names, scores))
print(paired)
# Output: [('Alice', 85), ('Bob', 90), ('Charlie', 95)]
```
