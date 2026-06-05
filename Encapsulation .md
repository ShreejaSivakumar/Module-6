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
