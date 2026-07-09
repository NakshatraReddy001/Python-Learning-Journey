# DAY 1: BASICS

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


### DAY 2 : STRINGS AND SEQUENTIAL DATATYPES

#### 1. Strings (`str`)

- **Def**: Text wrapped in `' '`, `" "`, or `''' '''` (multi-line). Immutable (cannot change after creation).
- **Slicing**: `[start:end]` (excludes end).
  - `text = "Python"` → `text[0:4]` is `'Pyth'`.
- **Indexing**: Starts at `0`. Negative indexing starts from the back (`-1` = last item).
- **Core Methods**:
  - `.upper()` / `.lower()` → Changes case.
  - `.strip()` → Trims outer whitespace.
  - `.replace(old, new)` → Replaces text.
  - `.split()` → Splits text into a List on spaces.
- **Formatting**: `f"Hello {name}"` (f-strings) or `"{}".format(name)`.

#### 2. Lists (`list`)

- **Def**: Ordered, Mutable, and allows mixed data types. Written with `[]`.
- **Core Methods**:
  - `.append(x)` → Adds `x` to end.
  - `.insert(i, x)` → Inserts `x` at index `i`.
  - `.extend([...])` → Merges with another list.
  - `.remove(x)` → Removes first occurrence of value `x`.
  - `.pop(i)` → Removes item by index `i`.
  - `.sort()` → Sorts list elements.

#### 3. Tuples (`tuple`)

- **Def**: Ordered but strictly Immutable (read-only list). Written with `()`.
- **Core Methods**:
  - `.count(x)` → Counts occurrences of `x`.
  - `.index(x)` → Returns index position of `x`.

#### 4. Sets (`set`)

- **Def**: Unordered collection of Unique elements (duplicates auto-removed). Written with `{}`.
- **Core Methods**:
  - `.add(x)` → Adds an element.
  - `.remove(x)` (errors if missing) vs. `.discard(x)` (no error if missing).
- **Set Math**:
  - `.union(s)` → Combines all items from both sets.
  - `.intersection(s)` → Gets items common to both sets.
  - `.difference(s)` → Gets items in first set but not in `s`.

#### 5. Dictionaries (`dict`)

- **Def**: Mapped key-value pairs (`{key: value}`). Keys must be unique.
- **Core Methods**:
  - `.get(key)` → Safely retrieves a value; returns `None` if key isn't found.
  - `.keys()` → Returns all dictionary keys.
  - `.values()` → Returns all dictionary values.
  - `.items()` → Returns all key-value pairs as a collection of tuples.
  - `.update({key: val})` → Updates or adds key-value pairs.
  - `.pop(key)` → Deletes pair using its key.

