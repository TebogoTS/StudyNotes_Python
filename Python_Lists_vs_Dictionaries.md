### Lists vs. Dictionaries in Python:

1. **Lists**:
   - Use **square brackets** (`[ ]`).
   - Store items in an **ordered** sequence.
   - Each item is accessed by its **index**, starting at 0.
   - Example:
     ```python
     spells = ["Riddikulus!", "Wingardium Leviosa!", "Avada Kedavra!"]
     print(spells[1])  # Outputs: Wingardium Leviosa!
     ```

2. **Dictionaries**:
   - Use **curly brackets** (`{ }`).
   - Store items as **key-value pairs**, where:
     - Keys are **unique** and used to look up values.
     - Values can be anything: strings, numbers, lists, other dictionaries, etc.
   - Items are accessed by their **key**, not by an index.
   - Example:
     ```python
     quotes = {
         "Moe": "A wise guy, huh?",
         "Larry": "Ow!",
         "Curly": "Nyuk nyuk!",
     }
     print(quotes["Larry"])  # Outputs: Ow!
     ```

### Syntax Highlights:
- **Lists**:
  - `[item1, item2, item3]`
- **Dictionaries**:
  - `{key1: value1, key2: value2, key3: value3}`

### Why Use Dictionaries?
- Dictionaries are often more convenient than lists when you need to **map a key to a value**.
- They allow for **fast lookups** by name, rather than relying on numeric indices.
- They can be used to store structured data, making your code more readable and maintainable.

