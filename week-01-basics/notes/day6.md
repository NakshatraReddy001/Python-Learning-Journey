# Day 6: NumPy 

NumPy (Numerical Python) is the core library for scientific computing in Python. It provides high-performance multidimensional array objects and tools to work with them.

## 1. What is a NumPy Array?

- **Definition**: A grid of values, all of the same type (homogeneous), indexed by a tuple of non-negative integers.
- **Why NumPy over Lists?**:
  - **Speed**: NumPy arrays are written in C, making them significantly faster than Python lists.
  - **Memory**: Consumes less memory.
  - **Convenience**: Allows element-wise operations (vectorization) without writing loops.

## 2. Creating NumPy Arrays

- **From Python Lists**: `np.array([1, 2, 3])`
- **Built-in Initializers**:
  - `np.zeros(shape)` → Fills with zeros (e.g., `np.zeros((2, 3))`).
  - `np.ones(shape)` → Fills with ones.
  - `np.full(shape, fill_value)` → Fills with a constant value.
  - `np.arange(start, stop, step)` → Creates sequence of numbers (similar to Python's `range`).
  - `np.linspace(start, stop, num)` → Creates `num` evenly spaced values over a specified interval.
  - `np.eye(n)` → Creates an n × n identity matrix.
  - `np.random.random(shape)` → Fills with random floats between 0 and 1.

## 3. Array Attributes

Every array has properties that describe its structure:

- `.ndim`: Number of dimensions (axes).
- `.shape`: A tuple of integers showing the size of the array in each dimension.
- `.size`: Total number of elements in the array.
- `.dtype`: Data type of the elements inside the array.

## 4. Indexing & Slicing

- **1D Arrays**: Works exactly like standard Python lists: `arr[start:stop:step]`.
- **Multi-dimensional Arrays**: Use comma-separated indices to select elements from each dimension: `arr[row, column]`.
  - Example: `arr[0, 2]` selects the element in the first row, third column.
  - Slicing multidimensional arrays: `arr[0:2, 1:3]` extracts a subarray consisting of rows 0–1 and columns 1–2.

## 5. Array Reshaping & Manipulation

- `.reshape(new_shape)`: Changes the layout of an array without changing its data (e.g., converting a 1D array of 6 elements into a 2 × 3 array).
- `.flatten()` or `.ravel()`: Collapses a multi-dimensional array into a single 1D array.
- `.T` (Transpose): Flips the dimensions (rows become columns and vice versa).

## 6. Vectorized Operations & Broadcasting

- **Element-wise Arithmetic**: Operations like `+`, `-`, `*`, and `/` are applied element-by-element automatically (no loops needed).
  - Example: `arr * 2` multiplies every element inside `arr` by 2.
- **Broadcasting**: A powerful feature that allows mathematical operations to run on arrays of different shapes (e.g., adding a 1D array to a 2D array).

## 7. Statistical & Mathematical Functions

NumPy provides fast built-in mathematical tools:

- **Sum & Product**: `np.sum(arr)`, `np.prod(arr)`.
- **Statistics**: `np.mean(arr)` (Average), `np.median(arr)`, `np.std(arr)` (Standard Deviation).
- **Min/Max**: `np.min(arr)` / `np.max(arr)`, and `np.argmin(arr)` / `np.argmax(arr)` (returns indices of the min/max values).
- **Axis Operations**: You can specify `axis=0` (columns) or `axis=1` (rows) to perform statistics across a specific direction.
