# Python Introduction

Python is a high-level programming language with a simple and readable syntax. It is commonly used for web development, data analysis, automation and machine learning.

## Installation

Open your Terminal and write the command.

```bash
sudo apt install python3
```

- Verify the installation:

```bash
python3 --version
```

## First Program

In python `print` is a inbuilt function to display the output.

```bash
 print("Hello, World!") 
 ```

 ## Python Indentation

 - Indentation refers to the spaces at the beginning of a code line.

- Python uses indentation to indicate a block of code.

### Example

```bash
if 5 > 2:
    print("Five is greater than two!")
```

## Python Variables

In Python, variables are created when you assign a value to it.

### Example
```bash
x = 5
y = "Hello, World!"
```
Assign Multiple Values:

```bash
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

## Data Types

Python has the following data types:


| Type Category      | Data Types                           |
|--------------------|--------------------------------------|
| Text Type          | str                                  |
| Numeric Types      | int, float, complex                  |
| Sequence Types     | list, tuple, range                   |
| Mapping Type       | dict                                 |
| Set Types          | set, frozenset                       |
| Boolean Type       | bool                                 |
| Binary Types       | bytes, bytearray, memoryview         |
| None Type          | NoneType                             |


### Getting the Data Type

You can get the data type of any object by using the `type()` function:

```bash
x = 5
print(type(x))
```

### Specific Data Type
If you want to specify the data type, you can use the following constructor functions:

```bash
x = str("Hello World")
x = int(20)
x = float(20.5)
x = list(("apple", "banana", "cherry"))
x = tuple(("apple", "banana", "cherry"))
x = range(6)
x = dict(name="John", age=36)
x = set(("apple", "banana", "cherry"))
```

