# Day 3: Operators

## 1. Arithmetic Operators

Used to perform mathematical computations.

- **Addition (`+`)**: Adds values together (e.g., `5 + 3 = 8`).
- **Subtraction (`-`)**: Subtracts the second value from the first (e.g., `10 - 4 = 6`).
- **Multiplication (`*`)**: Multiplies values (e.g., `6 * 2 = 12`).
- **Division (`/`)**: Performs standard float division (e.g., `15 / 3 = 5.0`).
- **Floor Division (`//`)**: Divides and rounds down to discard the remainder (e.g., `15 // 3 = 5`).
- **Modulo (`%`)**: Returns only the division remainder (e.g., `17 % 4 = 1`).
- **Exponentiation (`**`)**: Raises a base number to a power (e.g., `2 ** 4 = 16`).

## 2. Assignment Operators

Used to assign and modify values in variables.

- `=`: Basic assignment (e.g., `x = 5`).
- `+=`: Add and assign (e.g., `x += 3` is equivalent to `x = x + 3`).
- `-=`: Subtract and assign (e.g., `x -= 3` is equivalent to `x = x - 3`).
- `*=`: Multiply and assign (e.g., `x *= 3` is equivalent to `x = x * 3`).
- `/=`: Divide and assign (e.g., `x /= 3` is equivalent to `x = x / 3`).
- `//=`: Floor divide and assign (e.g., `x //= 3` is equivalent to `x = x // 3`).
- `%=`: Modulo and assign (e.g., `x %= 3` is equivalent to `x = x % 3`).
- `**=`: Exponentiate and assign (e.g., `x **= 3` is equivalent to `x = x ** 3`).

## 3. Comparison Operators

Used to compare two values; always returns a boolean (`True` or `False`).

- `==`: Equal to (e.g., `5 == 5` → `True`).
- `!=`: Not equal to (e.g., `7 != 5` → `True`).
- `>`: Greater than (e.g., `10 > 5` → `True`).
- `<`: Less than (e.g., `3 < 10` → `True`).
- `>=`: Greater than or equal to.
- `<=`: Less than or equal to.

## 4. Logical Operators

Used to combine conditional or comparison statements.

- `and`: Returns `True` only if both conditions are true.
- `or`: Returns `True` if at least one condition is true.
- `not`: Reverses the logical state (turns `True` into `False` and vice versa).

## 5. Membership Operators

Used to verify if an item exists within a sequence like a string, list, or tuple.

- `in`: Returns `True` if the specified value is found in the sequence.
- `not in`: Returns `True` if the specified value is absent from the sequence.

## 6. Identity Operators

Used to evaluate whether two variables share the exact same reference location in memory.

- `is`: Returns `True` if variables point to the same underlying object.
- `is not`: Returns `True` if variables point to completely separate memory objects.

> **Note:** `==` evaluates whether values are equal, whereas `is` evaluates if the memory addresses match.
