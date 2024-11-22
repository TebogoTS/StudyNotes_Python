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

This table serves as a quick reference guide for understanding Python's basic types, their mutability, and how they behave in practice!
