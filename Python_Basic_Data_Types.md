Here’s a summary of the basic data types in Python as outlined in **Table 2-1**, along with explanations for each column:

---

### **Python’s Basic Data Types**

| **Name**       | **Type**      | **Mutable?** | **Examples**                                | **Chapter** |
|-----------------|--------------|--------------|---------------------------------------------|-------------|
| **Boolean**     | `bool`       | No           | `True`, `False`                             | Chapter 3   |
| **Integer**     | `int`        | No           | `47`, `25000`, `25_000`                     | Chapter 3   |
| **Floating Point** | `float`   | No           | `3.14`, `2.7e5`                             | Chapter 3   |
| **Complex**     | `complex`    | No           | `3j`, `5 + 9j`                              | Chapter 22  |
| **Text String** | `str`        | No           | `'alas'`, `"alack"`, `'''a verse attack'''` | Chapter 5   |
| **List**        | `list`       | Yes          | `['Winken', 'Blinken', 'Nod']`              | Chapter 7   |
| **Tuple**       | `tuple`      | No           | `(2, 4, 8)`                                 | Chapter 7   |
| **Bytes**       | `bytes`      | No           | `b'ab\xff'`                                 | Chapter 12  |
| **ByteArray**   | `bytearray`  | Yes          | `bytearray(...)`                            | Chapter 12  |
| **Set**         | `set`        | Yes          | `set([3, 5, 7])`                            | Chapter 8   |
| **Frozen Set**  | `frozenset`  | No           | `frozenset(['Elsa', 'Otto'])`               | Chapter 8   |
| **Dictionary**  | `dict`       | Yes          | `{'game': 'bingo', 'dog': 'dingo', 'drummer': 'Ringo'}` | Chapter 8 |

---

### **Explanation of Each Column**

1. **Name**:
   - A human-readable name for the type, e.g., **Boolean**, **Integer**, **Text String**, etc.

2. **Type**:
   - The corresponding Python type name, e.g., `bool`, `int`, `str`, `list`.

3. **Mutable?**:
   - Indicates whether an instance of this type can be modified after creation:
     - **Yes**: The object can be changed in place (e.g., `list`, `set`, `dict`).
     - **No**: The object is immutable, meaning its value cannot be altered after creation (e.g., `int`, `str`, `tuple`).

4. **Examples**:
   - Literal examples that represent values of this type in Python code.

5. **Chapter**:
   - Points to the chapter where the type is covered in detail.

---

### **Key Concepts**

#### **Mutable vs Immutable**
- **Immutable Types** (e.g., `int`, `str`, `tuple`):
  - Cannot be changed after creation.
  - Example:
    ```python
    x = 47
    x += 1  # This creates a new integer object with value 48. `x` now points to the new object.
    ```

- **Mutable Types** (e.g., `list`, `dict`, `set`):
  - Can be modified in place.
  - Example:
    ```python
    fruits = ['apple', 'banana']
    fruits.append('cherry')  # Modifies the original list.
    print(fruits)  # Output: ['apple', 'banana', 'cherry']
    ```

---

### **Examples of Use**

1. **Boolean**:
   ```python
   is_active = True
   print(type(is_active))  # Output: <class 'bool'>
   ```

2. **Integer**:
   ```python
   age = 25_000  # Underscores improve readability
   print(type(age))  # Output: <class 'int'>
   ```

3. **Floating Point**:
   ```python
   pi = 3.14
   scientific = 2.7e5  # Scientific notation
   print(type(pi))  # Output: <class 'float'>
   ```

4. **Complex**:
   ```python
   z = 3 + 4j
   print(type(z))  # Output: <class 'complex'>
   ```

5. **Text String**:
   ```python
   poem = '''Roses are red,
   Violets are blue.'''
   print(type(poem))  # Output: <class 'str'>
   ```

6. **List**:
   ```python
   numbers = [1, 2, 3]
   numbers.append(4)  # Modifies the list
   print(numbers)  # Output: [1, 2, 3, 4]
   ```

7. **Tuple**:
   ```python
   coords = (10, 20)
   # coords[0] = 15  # TypeError: 'tuple' object does not support item assignment
   ```

8. **Bytes and ByteArray**:
   ```python
   b = b'ab\xff'
   print(type(b))  # Output: <class 'bytes'>

   ba = bytearray(b)
   ba[1] = 99
   print(ba)  # Output: bytearray(b'ac\xff')
   ```

9. **Set**:
   ```python
   items = {1, 2, 3}
   items.add(4)  # Modifies the set
   print(items)  # Output: {1, 2, 3, 4}
   ```

10. **Frozen Set**:
    ```python
    frozen = frozenset(['Elsa', 'Otto'])
    # frozen.add('Anna')  # AttributeError: 'frozenset' object has no attribute 'add'
    ```

11. **Dictionary**:
    ```python
    data = {'key': 'value'}
    data['key'] = 'new_value'  # Modifies the dictionary
    print(data)  # Output: {'key': 'new_value'}
    ```

---

### Study Notes: Chapter 2 - Data: Types, Values, Variables, and Names

---

#### **Key Concepts**

1. **Data Representation in Computers**:
   - Computers store data as bits (0s and 1s).
   - These bits can represent different data types (e.g., numbers, text, code) depending on interpretation.

2. **Python Objects**:
   - All Python data types are objects.
   - Objects have:
     - **Type**: Determines what the object can do.
     - **Unique ID**: Identifies the object in memory.
     - **Value**: The data inside the object.
     - **Reference Count**: Tracks how many variables reference the object.

3. **Memory Model**:
   - Visualize memory as shelves filled with boxes (objects).
   - Boxes have labels (type and value) and are referenced by variable names.

4. **Data Types in Python**:
   - **Immutable Types**: Values cannot change after creation (e.g., int, float, tuple, str).
   - **Mutable Types**: Values can be modified (e.g., list, dict, set).
   - Python strongly types variables—an object’s type doesn’t change even if mutable.

5. **Variables**:
   - Variables are *names* pointing to objects.
   - Names are case-sensitive and must follow specific naming rules.

6. **Assignment and Reassignment**:
   - `=` assigns a value to a variable, but it’s not the same as mathematical equality.
   - Reassigning a variable makes it reference a new object, not modify the original.

7. **Reference Behavior**:
   - Variables can reference the same object.
   - Immutable objects: Value remains unchanged.
   - Mutable objects: Changes affect all variables referencing the object.

8. **Garbage Collection**:
   - Python automatically manages memory.
   - Objects with zero references are garbage-collected.

9. **Choosing Variable Names**:
   - Use meaningful names for clarity and maintenance.
   - Balance between brevity (short names) and clarity (descriptive names).

---

#### **Examples**

1. **Assigning and Printing Variables**:
   ```python
   prince = 99
   print(prince)  # Output: 99
   ```

2. **Checking Data Types**:
   ```python
   type(5)         # <class 'int'>
   type(2.0)       # <class 'float'>
   type(5 + 2.0)   # <class 'float'>
   ```

3. **Immutable vs Mutable Objects**:
   - Immutable Example:
     ```python
     x = 5
     y = x
     x = 10
     print(x)  # Output: 10
     print(y)  # Output: 5
     ```
   - Mutable Example:
     ```python
     a = [1, 2, 3]
     b = a
     a[0] = 99
     print(a)  # Output: [99, 2, 3]
     print(b)  # Output: [99, 2, 3]
     ```

4. **Simultaneous Assignment**:
   ```python
   x = y = z = 42
   print(x, y, z)  # Output: 42 42 42
   ```

5. **Checking Types with `isinstance()`**:
   ```python
   isinstance(5, int)    # True
   isinstance(2.0, int)  # False
   ```

---

#### **Things to Try**

1. Assign `99` to the variable `prince` and print it:
   ```python
   prince = 99
   print(prince)  # Output: 99
   ```

2. Check the type of the value `5`:
   ```python
   print(type(5))  # <class 'int'>
   ```

3. Check the type of `2.0`:
   ```python
   print(type(2.0))  # <class 'float'>
   ```

4. Evaluate the type of the expression `5 + 2.0`:
   ```python
   print(type(5 + 2.0))  # <class 'float'>
   ```

---

#### **Takeaways**

- Python’s flexible data handling abstracts away low-level memory management.
- Understanding Python’s data model and variable behavior is critical for efficient programming.
- Thoughtful variable naming improves code readability and maintainability.
