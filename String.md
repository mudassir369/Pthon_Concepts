# STRING

Strings in python are surrounded by either single quotation marks, or double quotation marks.

- `'hello'` is the same as `"hello"`.

```bash
 a = "Hello"
print(a)  #Hello
```

## Multiline Strings

You can assign a multiline string to a variable by using three quotes.

```bash
 a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a) 
```

Like many other popular programming languages, strings in Python are arrays of unicode characters.

```bash
a = "Hello, World!"
print(a[1])   # e
```

## String Length

To get the length of a string, use the `len()` function.

```bash
a = "Hello, World!"
print(len(a))  # 13
```

## Check String

To check if a certain phrase or character is present in a string, we can use the keyword `in`.

```bash
 txt = "The best things in life are free!"
print("free" in txt)    # True
```
OR

```bash
txt = "The best things in life are free!"
if "free" in txt:                           # Condition is true
  print("Yes, 'free' is present.")
```

## Check if NOT

To check if a certain phrase or character is NOT present in a string, we can use the keyword not in.

```bash
txt = "The best things in life are free!"
print("expensive" not in txt)   # True
```

## Slicing In Strings

- You can return a range of characters by using the slice syntax.
- Specify the start index and the end index, separated by a colon, to return a part of the string.

```bash
b = "Hello, World!"
print(b[2:5])   # llo
```

## Negative Indexing

Use negative indexes to start the slice from the end of the string: 

```bash
b = "Hello, World!"
print(b[-5:-2])     # orl
```

## String Methods

**Most popular** and **commonly used** string methods in Python.

### Upper Case

- The `upper()` method returns the string in upper case.

```bash
a = "Hello, World!"
print(a.upper())    # HELLO, WORLD!
```
### Lower Case
- The `lower()` method returns the string in lower case.

```bash
 a = "Hello, World!"
print(a.lower())    # hello, world!
```

### Remove Whitespace

- The `strip()` method remove any whitespace from the begining or the end.

```bash
a = " Hello, World! "
print(a.strip())    # "Hello, World!"
```

### Replace String

- The `replace()` method replaces a string with another string.
```bash
a = "Hello, World!"
print(a.replace("H", "J"))  # Jello, World!
```

### Split String

- The `split()` method splits the string into substrings if it finds instances of the separator.

```bash
a = "Hello, World!"
print(a.split(","))   # ['Hello', ' World!']
```

### Title 

- The `title()` method capitalizes first letter of each word.

```bash
a = "hello, world!"
print(a.title())    # Hello, World!
```

### Capitalize

- The `capitalize()` method capitalize first character of sentance.

```bash
a = "hello world!"
print(a.capitalize())   # Hello world!
```

### Swapcase

- The `swapcase()` method swap uppercase to lowercase and vice versa.

```bash
a = "Hello"
print(a.swapcase())     # hELLO
```

### Searching and Finding

| Method         | Description                     | Example                             |
|----------------|---------------------------------|-------------------------------------|
| `find()`       | Return index of first occurrence| `"hello".find("e")` # 1             |
| `rfind()`      | Find from right side            | `"hello".rfind("l")` # 3            |
| `index()`      | Same as find but gives error if not found| `"hello".index("e")` # 1   |
| `count()`      | Count occurrences of char       | `"hello".count("l")` # 2            |
| `startswith()` | Checks start                    | `"hello".startswith("he")` # True   |
| `endswith()`   | Checks end                      | `"hello".endswith("lo")` # True     |


### Replacing and Modifying

| Method         | Desscription                    | Example                             |
|----------------|---------------------------------|-------------------------------------|
| `replace(old,new)` | Replaces substring          | `"hello".replace("l","x")` # hexxo  |
| `strip()`      | Removes spaces both sides       | `" hi ".strip()` # "hi"             |
| `lstrip()`     | Removes left spaces             | `" hi ".lstrip()` # "hi "           |
| `rstrip()`     | Removes right spaces            | `" hi ".rstrip()` # " hi"           |

---

### Checking Method (Return True/False)

| Method          | Description              |
|-----------------|--------------------------|
| `isalpha()`     | Only letters             |
| `isdigit()`     | Only Digits              |
| `isalnum()`     | Letters + Digits         |
| `isspace()`     | Only spaces              |
| `islower()`     | All lowercase            |
| `isupper()`     | All uppercase            |
| `istitle()`     | Title case               |

---
