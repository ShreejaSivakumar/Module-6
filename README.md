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


------------------------------------------------------------------------------------------------------------
# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    def __init__(self, length, breadth): 
        self.__length = length 
        self.__breadth = breadth 
        self.display_values()

    def display_values(self):
        print(f"Length: {self.__length}")
        print(f"Breadth: {self.__breadth}")
rect = Rectangle(10, 5)
```
<img width="618" height="262" alt="Screenshot 2026-06-05 211934" src="https://github.com/user-attachments/assets/f1e769e9-2c18-4c84-945f-104731dea6d2" />

## Output
<img width="215" height="83" alt="Screenshot 2026-06-05 211937" src="https://github.com/user-attachments/assets/ca971a1b-21fb-44ae-a29d-63b7ab20a4db" />

## Result
Thus To implement Encapsulation in Python by defining a class Rectangle with private member variables __length and __breadth. Hence the code has been executed successfully.


------------------------------------------------------------------------------------------------------

# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:
```
class Fish:
    def type(self): 
        print("fish")

class Shark(Fish):
    def type(self): 
        print("shark") 
obj_goldfish = Fish() 
obj_hammerhead = Shark() 
for fish in (obj_goldfish, obj_hammerhead):
    fish.type()
```
<img width="596" height="291" alt="Screenshot 2026-06-05 212054" src="https://github.com/user-attachments/assets/12c2b1b4-f244-45e9-9073-c61b7b74a714" />

## OUTPUT
<img width="162" height="62" alt="Screenshot 2026-06-05 212058" src="https://github.com/user-attachments/assets/389210be-388a-482c-aa0b-461ffa6abde0" />

## RESULT
Thus To write a Python program that demonstrates class inheritance by creating a parent class Fish with a method type, and a child class Shark that overrides the type method. Hence the code has been executed successfully.

--------------------------------------------------------------------------------------------------------

# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

---

## 💻 Program
```
class A:
    def __init__(self, a):
        self.a = a
    def __lt__(self, o):
        if self.a < o.a:
            return "ob1 is less than ob2"
        else:
            return "ob2 is less than ob1"
ob1 = A(30)
ob2 = A(50)
print(ob1 < ob2)

```
<img width="586" height="282" alt="Screenshot 2026-06-05 212212" src="https://github.com/user-attachments/assets/248e2cc1-c853-4a5b-88c1-fd2a887f8d31" />

## Output
<img width="317" height="47" alt="Screenshot 2026-06-05 212215" src="https://github.com/user-attachments/assets/7dc2763b-cfe9-4061-9b8f-edf7571dfb9c" />


## Result
Thus To write a Python program that demonstrates operator overloading by overloading the less than (<) operator using a custom class. Hence the code has been executed successfully.

-------------------------------------------------------------------------------------------------------
# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

---

## 💻 Program
```
class Beans:
    def type(self): 
        print("Vegetable")
    def color(self):
        print("Green")
class Mango:
    def type(self): 
        print("Fruit")
    def color(self):
        print("Yellow")
def func(obj) : 
    obj.type() 
    obj.color()
bean_obj = Beans()
mango_obj = Mango()
func(bean_obj) 
func(mango_obj)
```
<img width="338" height="415" alt="Screenshot 2026-06-05 212323" src="https://github.com/user-attachments/assets/245fe60b-cb15-4444-8458-efc5b6cb1e88" />


## Output
<img width="171" height="137" alt="Screenshot 2026-06-05 212327" src="https://github.com/user-attachments/assets/a777c94d-0aac-4459-a14e-77eb362fa704" />



## Result
Thus To create two specific classes — Beans and Mango. Then, create a generic function that can accept any object and determine its type (Fruit or Vegetable) and color, using polymorphism. Hence the code has been executed successfully.

--------------------------------------------------------------------------------------------------------



