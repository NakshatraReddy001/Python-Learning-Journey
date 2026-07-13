## DAY 2 : STRINGS AND SEQUENTIAL DATATYPES

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
