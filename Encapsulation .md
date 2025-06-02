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
      class Rectangle:
          def __init__(self, length, breadth):
              # Step 1 & 2: Private attributes
              self.__length = length
              self.__breadth = breadth
      
          def display(self):
              # Step 3: Accessing private variables inside the class
              print(f"Length: {self.__length}")
              print(f"Breadth: {self.__breadth}")
      
      # Step 4: Instantiate the object
      rect = Rectangle(10, 5)
      rect.display()
      
      # Trying to access private variables directly will raise AttributeError:
      # print(rect.__length)  # Uncommenting this will cause an error


## Output
Length: 10
Breadth: 5

## Result
The private members __length and __breadth are encapsulated within the class. They are accessible inside class methods but not directly accessible from outside the class (demonstrating encapsulation).
