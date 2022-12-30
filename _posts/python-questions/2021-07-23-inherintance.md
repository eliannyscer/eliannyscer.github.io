---
title: "What mean Inheritance"
tags:
  - Python questions
---

Inheritance is the `capability` of one class to `derive` or inherit the `properties` from another class. It provides code reusability, makes it easier to create and maintain an application. The class from which we are inheriting is called `base or parent-class` and the class that is inherited is called a `derived / child class`.

`Example` - Base class:

```python
class Person:
  def __init__(self, f_name, l_name):
    self.first_name = f_name
    self.last_name = l_name

  def print_name(self):
    print(self.first_name, self.last_name)

#Use the Person class to create an object, and then execute the print_name method:

x = Person("Ellie", "Johnson")
x.print_name() 

# Output:
Ellie Johnson
```

`Example` - Derived class

To create a class that inherits the functionality from another class, send the parent class as a parameter when creating the child class:

```python
 class Student(Person):
  pass 
```

```python
class Person:
  def __init__(self, f_name, l_name):
    self.first_name = f_name
    self.last_name = l_name

  def print_name(self):
    print(self.first_name, self.last_name)

class Student(Person):
  pass

x = Student("Karl", "Olsen")
x.print_name()

# Output:
Karl Olsen
```

## References

[Inheritance](https://www.geeksforgeeks.org/inheritance-in-python/)

[Example](https://www.w3schools.com/python/python_inheritance.asp)

[The four pillars of object orientation](https://www.freecodecamp.org/news/four-pillars-of-object-oriented-programming/)
