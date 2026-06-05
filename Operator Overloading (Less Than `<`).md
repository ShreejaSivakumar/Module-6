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
