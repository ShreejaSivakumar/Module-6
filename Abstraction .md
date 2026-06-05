# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math
class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass
class Rectangle(Shape):
    def __init__(self, length, width):
        self.length = length
        self.width = width
    def calculate_area(self):
        return self.length * self.width
class Circle(Shape):
    def __init__(self, radius):
        self.radius = radius
    def calculate_area(self):
        return math.pi * self.radius * self.radius
rect = Rectangle(10, 5)
circle = Circle(7)
print("Rectangle Area:", rect.calculate_area())
print("Circle Area:", circle.calculate_area())

```
<img width="643" height="521" alt="Screenshot 2026-06-05 211452" src="https://github.com/user-attachments/assets/e3c8e862-9172-417b-91bf-cd6e64d9d71c" />

## Output

<img width="378" height="93" alt="Screenshot 2026-06-05 211457" src="https://github.com/user-attachments/assets/7cb517c9-f0e1-4f25-bc6b-73870b8f1077" />

## Result
Thus To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle. Hence the code has been executed successfully.
