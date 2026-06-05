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
