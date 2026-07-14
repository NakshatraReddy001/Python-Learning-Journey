# Day 4: Conditional Statements and Loops

## 1. Conditional Statements

Conditional statements allow Python to make decisions and execute specific blocks of code only when certain conditions are met.

### A. `if` Statement

- **Def**: Executes a block of code only if the specified condition evaluates to `True`.
- **Example**:
```python
age = 18
if age >= 18:
    print("You are eligible to vote.")
```

### B. `if-else` Statement

- **Def**: Provides an alternative block of code (`else`) that runs if the `if` condition evaluates to `False`.
- **Example**:
```python
if num % 2 == 0:
    print("Even number")
else:
    print("Odd number")
```

### C. `if-elif-else` Statement

- **Def**: Extends the `if-else` structure with `elif` (else if) clauses to test multiple independent conditions sequentially.
- **Example**:
```python
if score >= 90:
    grade = 'A'
elif score >= 80:
    grade = 'B'
else:
    grade = 'F'
```

### D. Nested `if-else` Conditions

- **Def**: Placed inside another `if` or `else` block to build complex, multi-layered decision-making paths.
- **Example**:
```python
if age >= 18:
    if income >= 25000:
        print("Eligible for a loan.")
    else:
        print("Income too low.")
```

### E. Ternary Operator

- **Def**: A compact, one-line shorthand syntax for writing simple `if-else` structures.
- **Example**:
```python
status = "Adult" if age >= 18 else "Minor"
```

## 2. Loops

Loops are used to perform repetitive tasks and process collections of items efficiently.

### A. `for` Loop

- **Def**: Used to iterate over a sequence (like a list, tuple, or string) and repeatedly run a block of code for each item.
- **Example**:
```python
fruits = ['apple', 'banana', 'orange']
for fruit in fruits:
    print(fruit)
```

### B. `while` Loop

- **Def**: Repeatedly runs a block of code as long as a specified condition evaluates to `True`.
- **Essential Rule**: Always include logic within the loop that eventually makes the condition `False`; otherwise, it results in an infinite loop that runs indefinitely.
- **Example**:
```python
count = 0
while count < 5:
    print("Count:", count)
    count += 1
```

### C. Python "Do-While" Loop Logic

- **The Catch**: Python does not have a built-in `do-while` loop.
- **Workaround**: You can achieve equivalent behavior using a `while True` loop paired with an internal condition and a `break` statement to exit.
- **Example**:
```python
count = 0
while True:
    print("Count:", count)
    count += 1
    if count >= 5:
        break
```
