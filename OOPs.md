# PYTHON OOP

- OOP stants for **Object Oriented Programming**.
- Python is an object oriented language, allowing you to structure your code using classes and objects for better organization and reusability.

## Advanyages of OOP

- Provides a clear structure to programs.
- Makes code easier to maintain, reuse and debug.
- Helps keep your code DRY (Don't Repeat Yourself).
- Whene you create an object from a class, it inherits all the variables and functions defined inside that class.

## Python Classes and Objects

- Almost everything in Python is an object, with its properties and methods.
- A Class is like an object constructor, or a **blueprint** for creating objects.

### Create a Class

To create a class, yse the keyword `class`.

```bash
class MyClass:
    x = 5
```

### Create Object

Now we can use the class named MyClass to create objects.

Create an object named p1, and print the value of x:

```bash
p1 = MyClass()
print(p1.x)
```

### Multiple Objects

You can create multiple objects from the same class.

```bash
p1 = MyClass()
p2 = MyClass()

print(p1.x)
print(p2.x)
```
---

## __init__() Method

- All classes have a built-in method called `__init__()`,which is always executed when the class in being initiated.

- The `__init__()` method is used to assign values to object properties, or to perform opetarions that are mecessary when the onject is being created.

### Example

```bash
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

p1 = Person("Mudassir", 24)

print(p1.name)  # Mudassir
print(p1.age)   # 24
```

## Self Parameter

- The `self` parameter is a reference to the current instance of the class.

- It is used to access properties and methods that belong to the class.

```bash
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def greet(self):
    print("Hello, my name is " + self.name)

p1 = Person("Emil", 25)
p1.greet() 
```
---

## Class Properties

- Properties are variables that belong to a class. They store data for each object created from the class.

```bash
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("Emil", 36)

print(p1.name)
print(p1.age) 
```
## Access Properties

- You can access object properties using dot(.) notation.

```bash
class Car:
  def __init__(self, brand, model):
    self.brand = brand
    self.model = model

car1 = Car("Toyota", "Corolla")

print(car1.brand)
print(car1.model) 
```

## Modify Properties

- You can modify the value of properties on objects.

```bash
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("Tobias", 25)
print(p1.age)

p1.age = 26
print(p1.age) 
```

---

