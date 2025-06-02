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
      from abc import ABC, abstractmethod
      import math
      
      # Step 2: Abstract Class
      class Shape(ABC):
          @abstractmethod
          def calculate_area(self):
              pass
      
      # Step 3: Rectangle subclass
      class Rectangle(Shape):
          def __init__(self, length=5, breadth=3):
              self.length = length
              self.breadth = breadth
      
          def calculate_area(self):
              return self.length * self.breadth
      
      # Step 4: Circle subclass
      class Circle(Shape):
          def __init__(self, radius=7):
              self.radius = radius
      
          def calculate_area(self):
              return math.pi * (self.radius ** 2)
      
      # Step 5: Create objects and call methods
      rect = Rectangle()
      circle = Circle()
      
      print(f"Area of Rectangle: {rect.calculate_area():.2f}")
      print(f"Area of Circle: {circle.calculate_area():.2f}")


## Output
Area of Rectangle: 15.00
Area of Circle: 153.94


## Result
The program defines an abstract class Shape with an abstract method calculate_area. Both Rectangle and Circle implement this method, calculating their respective areas correctly.
