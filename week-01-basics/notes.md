# Week 1: BASICS

## 1. Introduction & Setup

- **What is Python?**: A high-level, interpreted, general-purpose, beginner-friendly, and cross-platform programming language.
- **History**: Developed by Guido van Rossum in the 1980s. Python 3.x is the only currently maintained version.
- **Sanity Checks**:
  - Check version: `python --version`
  - Run test: `print("Hello, Python!")`

## 2. Python Syntax Rules & Indentation

- **Core Rules**: Code runs sequentially line-by-line. Statements end with a newline (semicolons are optional). Completely case-sensitive.
- **Indentation**: Uses whitespace instead of curly braces `{}` to outline blocks of code. Recommendation: 4 spaces per level.

## 3. Variables & Scope

- **Dynamic Typing**: You do not declare variable types explicitly; they are determined at runtime and can change as new data is assigned.
- **Multi-Word Styles**:
  - Camel Case: `myVariableName`
  - Pascal Case: `MyVariableName`
  - Snake Case: `my_variable_name`
- **Assignments**: Supports multi-variable assignment (`x, y = 1, 2`) and unpacking a collection (`std1, std2 = ["A", "B"]`).
- **Outputting (`print()`)**: Comma separates multiple values. Combining strings and numbers using `+` causes a runtime error.
- **Scope Rules**:
  - **Local**: Created inside functions; only accessible there.
  - **Global**: Created outside functions; accessible everywhere. Use the `global` keyword to modify a global variable inside a local block.

## 4. Naming Conventions & Comments

- **Valid**: Variable names in lowercase separated by underscores (`student_name`); constants in uppercase (`PI`); classes in PascalCase.
- **Invalid**: Names cannot begin with a digit or include special characters (except `_`), nor can they match Python keywords.
- **Comments**: Single-line comments begin with `#`. Multi-line notes are handled using unassigned triple quotes (`'''` or `"""`).
- **Escape Characters**: Backslash (`\`) inserts characters that are otherwise illegal within a string literal.

## 5. Data Types & Type Conversion

- **Built-In Types**: Use `type()` to evaluate a variable's data type. Common options include:
  - `str` (String): `"Alice"`
  - `int` (Integer): `21`
  - `float` (Decimal): `19.99`
  - `bool` (Boolean): `True` / `False`
- **Casting Functions**: Explicitly switch types using `int()`, `float()`, or `str()`.
- **Note**: Attempting to parse text that lacks numerical digits into an integer or float throws an error.
