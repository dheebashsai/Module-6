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
    # Step 1: Parent class Fish
    class Fish:
        def type(self):
            print("fish")
    
    # Step 2: Child class Shark overriding type method
    class Shark(Fish):
        def type(self):
            print("shark")
    
    # Step 3: Create Fish instance
    obj_goldfish = Fish()
    
    # Step 4: Create Shark instance
    obj_hammerhead = Shark()
    
    # Step 5 & 6: Loop through both objects and call type()
    for obj in (obj_goldfish, obj_hammerhead):
        obj.type()

## OUTPUT
fish
shark


## RESULT
The output shows method overriding where the Shark class overrides the type() method of the Fish class, demonstrating polymorphism in inheritance.
