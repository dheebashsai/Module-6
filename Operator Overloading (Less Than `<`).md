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
      class A:
          def __init__(self, a):
              self.a = a
      
          def __lt__(self, o):
              if self.a < o.a:
                  return "ob1 is less than ob2"
              else:
                  return "ob2 is less than ob1"
      
      # Create objects
      ob1 = A(10)
      ob2 = A(20)
      
      # Use < operator to trigger __lt__
      print(ob1 < ob2)  # Expected: ob1 is less than ob2
      
      # Also test the other way
      print(ob2 < ob1)  # Expected: ob2 is less than ob1


## Output
ob1 is less than ob2
ob2 is less than ob1


## Result
The < operator is overloaded by defining the __lt__() method, which compares the a values of two objects and returns a custom string message accordingly.
