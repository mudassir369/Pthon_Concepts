# SOLID Principles

SOLID is a set of 5 **Object-Oriented Design Principles** that help you write **clean, maintainable, and scalable code**.

## 1. S — Single Responsibility Principle (SRP)

- A class should have only one reason to change.

- One class = One responsibility.

### ❌ Bad Example:

```bash
class Report:
    def generate(self):
        pass

    def save_to_file(self):
        pass

    def send_email(self):
        pass
```
This class does:

- Generate report

- Save file

- Send email

Too many responsibilities ❌

### ✅ Good Example:

```bash
class ReportGenerator:
    def generate(self):
        pass

class ReportSaver:
    def save_to_file(self):
        pass

class EmailSender:
    def send_email(self):
        pass
```
✔ Each class has one responsibility.

---

## 2. O — Open/Closed Principle (OCP)

- Software should be **open for extension** but **closed for modification**.
- You should be able to add new features **without changing existing code**.

### ❌ Bad Example:

```bash
class Discount:
    def calculate(self, customer_type):
        if customer_type == "regular":
            return 10
        elif customer_type == "premium":
            return 20
```
If new customer type comes → modify class ❌

### ✅ Good Example:

```bash
class Discount:
    def calculate(self):
        pass

class RegularDiscount(Discount):
    def calculate(self):
        return 10

class PremiumDiscount(Discount):
    def calculate(self):
        return 20
```
Now we can extend without modifying original logic ✔

---

## 3. L — Liskov Substitution Principle (LSP)

- Child class should be able to replace parent class **without breaking the code**.

### ❌ Bad Example:

```bash
class Bird:
    def fly(self):
        pass

class Ostrich(Bird):
    def fly(self):
        raise Exception("Ostrich can't fly")
```
Ostrich cannot fly → breaks behavior ❌

### ✅ Good Example:

```bash
class Bird:
    pass

class FlyingBird(Bird):
    def fly(self):
        pass
```

Now only birds that fly inherit `FlyingBird` ✔

---

## 4. I — Interface Segregation Principle (ISP)

- Clients should not be forced to depend on methods they don’t use.
- Create smaller, specific interfaces instead of one large interface.

### ❌ Bad Example:

```bash
class Worker:
    def work(self):
        pass

    def eat(self):
        pass
```

Robot doesn’t eat ❌

### ✅ Better Design:

```bash
class Workable:
    def work(self):
        pass

class Eatable:
    def eat(self):
        pass
```

Now classes implement only what they need ✔

---

## 5. D — Dependency Inversion Principle (DIP)

- High-level modules should not depend on low-level modules.
- Both should depend on abstractions.
- Depend on interfaces, not concrete classes.

### ❌ Bad Example:

```bash
class MySQLDatabase:
    def connect(self):
        pass

class Application:
    def __init__(self):
        self.db = MySQLDatabase()
```

Application tightly coupled to MySQL ❌

### ✅ Better Design:

```bash
class Database:
    def connect(self):
        pass

class MySQLDatabase(Database):
    def connect(self):
        pass

class Application:
    def __init__(self, db: Database):
        self.db = db
```

Now we can pass MySQL, PostgreSQL, etc. ✔

---

## 🧠 Quick Summary Table

| Principle       |	Meaning                                  |
|-----------------|------------------------------------------|
| SRP             |	One class → One responsibility           |
| OCP             | Extend without modifying                 | 
| LSP             | Child must behave like parent            |
| ISP             | Small, specific interfaces               |
| DIP             |	Depend on abstraction, not concrete      |


## 🎯 Why SOLID is Important?

- Makes code scalable
- Easier to test
- Easier to maintain
- Reduces bugs
- Used in real-world system design

---

