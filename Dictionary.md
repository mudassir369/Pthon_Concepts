# DICTIONARY

- Dictionaries are used to stor data values in keys and values pairs.
- A dictionary is a collection which is ordered, changable and do not allow duplicate keys.
- Dictionaries are written with curly brackets and have keys and values.

### Example

```bash
dict1 = {
    "name" : "Mudassir",
    "age" : 24
}
print(dict1["age"]) # 24
```

## Important Method

### 1. Length

`len()` Print the number of items in the dictionary.

```bash
print(len(dict1))   # 2
print(dict1)    # {"name" : "Mudassir", "age" : 24}
```

### 2. Get Keys

`keys()` Get a list of the keys.

```bash
print(dict1.keys()) # ['brand', 'model', 'year']
```

Add a new item to the original dictionary.

```bash
dict1["add"] = "Moradabad"  #{"name":"Mudassir","age":24,"add":"Moradabad"}
```

### 3. Get Values

`values()` Get a list of the values.

```bash
dict1.values()  # ["Mudassir",24,"Moradabad"]
```

### 3. Change Values

YOu can change the value of a specific item by referring to its key name.

```bash
dict1["add"] = "UP, Moradabad"  # ["Mudassir",24,"UP, Moradabad"]
```

### 4. Pop Items

`pop()` method is used to remove the key name.

```bash
dict1.pop("add")
print(dict1)    # {"name":"Mudassir","age":24}
```

### 5. Pop Last Item

`popitem()` method used to pop last inserted item.

```bash
dict1.popitem()  # {"name":"Mudassir"}
```

### 6. Clear Method

`clear()` method empties the dictionary.

```bash
dict1.clear()  # {}
```

### 7. Copy Method

Make a copy of dictionary with the `copy()` method.

```bash
dict1 = {
    "Name" : "Mudassir",
    "Age" : 24
}

dict2 = dict1.copy()
print(dict2)  # {"Name" : "Mudassir", "Age" : 24}
```
---

