This Python script demonstrates the use of a **dictionary** and how to access its elements using keys.

---

### Code Breakdown:

```python
quotes = {
    "Moe": "A wise guy, huh?",
    "Larry": "Ow!",
    "Curly": "Nyuk nyuk!",
    }
```

1. **Dictionary Definition**:
   - `quotes` is a **dictionary** in Python. A dictionary is a collection of key-value pairs, defined with curly braces `{}`.
   - Each key is unique, and it is associated with a corresponding value.

2. **Key-Value Pairs**:
   - Keys in this dictionary are names of the Three Stooges: `"Moe"`, `"Larry"`, and `"Curly"`.
   - Values are the quotes associated with each Stooge:
     - `"Moe": "A wise guy, huh?"`
     - `"Larry": "Ow!"`
     - `"Curly": "Nyuk nyuk!"`

---

```python
stooge = "Curly"
```

3. **Variable Assignment**:
   - The variable `stooge` is assigned the string `"Curly"`. This will be used as the key to look up a value in the `quotes` dictionary.

---

```python
print(stooge, "says:", quotes[stooge])
```

4. **Accessing a Dictionary Value**:
   - `quotes[stooge]` retrieves the value associated with the key `"Curly"` from the dictionary. In this case, it retrieves `"Nyuk nyuk!"`.

5. **Printing the Output**:
   - The `print` function combines:
     - The value of the `stooge` variable (`"Curly"`)
     - The string `"says:"`
     - The value retrieved from the dictionary (`"Nyuk nyuk!"`)

---

### Output:
When you run this script, the output will be:

```
Curly says: Nyuk nyuk!
```

---

### Why Use a Dictionary?
Dictionaries are useful for associating related data (e.g., names and quotes in this example) and for quickly looking up values using keys. This makes them an essential data structure for many Python programs.
