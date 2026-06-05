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
