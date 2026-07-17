# Day 7: Exception Handling and File Handling

## 1. Python Exception Handling

Errors in Python are divided into two categories: Syntax Errors (bugs due to incorrect code structure that prevent execution) and Exceptions (internal events raised during runtime that disrupt the normal flow of the program).

### Common Exception Types

- `IOError`: Raised if a file cannot be opened.
- `ValueError`: Raised when a built-in function receives a wrong/inappropriate argument type.
- `ZeroDivisionError`: Raised when attempting to divide a number by zero.
- `ImportError`: Raised if Python is unable to find or load a specified module.
- `KeyboardInterrupt`: Raised when an unrequired key combination (like `Ctrl+C`) is pressed by the user.
- `EOFError`: Raised if the End-Of-File condition is hit without reading any data.

### The Core `try-except` Blocks

- **`try` block**: Used to enclose the code block that you want to check for potential runtime errors. It runs normally if no errors occur.
- **`except` block**: Contains code that automatically executes only if the preceding `try` block encounters an error.
- **`else` clause**: Placed after all `except` clauses. The code inside the `else` block executes only if the `try` block runs without raising any exceptions.
- **`finally` block**: A keyword block that always executes regardless of whether an exception was thrown, caught, or completely skipped. Ideal for cleanup actions.

### Syntax Structure Layout

```python
try:
    # Some Code that might crash
    print(12 / 1)
except ZeroDivisionError as ee:
    # Executed if division by zero occurs
    print(ee)
except Exception as e:
    # Executed for any other general error
    print(e)
else:
    # Executes if NO exceptions occur in the try block
    print("No exception in the above program")
finally:
    # ALWAYS executes no matter what
    print("Finally block completed.")
```

## 2. Python File Handling

File handling allows you to create, read, update, and delete files directly through Python scripts.

### Core Built-in File Operations

- **`open(filename, mode)`**: The primary built-in function used to interact with data files. It requires the file path and the mode of operation.
- **Common Access Modes**:
  - `'r'` (Read): Default mode. Opens a file for reading text; throws an error if the target file does not exist.
  - `'w'` (Write): Opens a file for writing. Overwrites existing contents or creates a brand new file if it doesn't exist.
  - `'a'` (Append): Opens a file to add content to the end without deleting current text; creates the file if missing.
  - `'x'` (Create): Explicitly creates a new file; returns a runtime error if the file already exists.

### Best Practices: The `with` Statement

Always manage files using a `with` statement block. It automatically closes the file object once the block finishes execution, preventing common memory leaks or file locking `IOError` issues.

### Code Example

```python
# Safely writing to a file
with open("notes.txt", "w") as file:
    file.write("Python is simple and versatile.")

# Safely reading from a file
with open("notes.txt", "r") as file:
    content = file.read()
    print(content)
```
