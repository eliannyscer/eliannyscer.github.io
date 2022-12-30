---
title: "Does python make use of access specifiers?"
tags:
  - Python questions
---

Yes, access specifiers or access modifiers in python programming are used to `limit the access` of class variables and class methods outside of class while implementing the concepts of inheritance. This can be achieved by: Public, Private and Protected keyword.

`Example:`

```python
#defining class Student
class Student:
    #constructor is defined
    def __init__(self, name, age, salary):
        self.age = age             # public Attribute
        self._name = name          # protected Attribute 
        self.__salary = salary     # private Attribute

    def _funName(self):            # protected method
        pass
 
    def __funName(self):           # private method
        pass

# object creation 
obj = Student("python",30,7777)
```

## Additional information

`Public access:` All the variables and methods (member functions) in python are by default public. Any instance variable in a class followed by the `self` keyword ie. `self.var_name` are public accessed.

`Private access:` Private members of a class (variables or methods) are those members which are `only accessible inside the class`. We cannot use private members outside of class. The syntax we follow to make any variable private is to write variable name followed by a double underscore (__) ie. `__varName`.

`Protected access:` This are restricted to be used only by the member functions and class members of the same class. And also it can be accessed or inherited by its derived class(child class). We can modify the values of protected variables of a class. The syntax we follow to make any variable protected is to write variable name followed by a single underscore (_) ie. `_varName`.

## Reference

[Access to specifiers](https://pythonlobby.com/access-specifiers-or-access-modifiers-in-python-programming-public-private-and-protected-keywords/)
