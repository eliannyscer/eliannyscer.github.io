---
title: "What is encapsulation in Python"
tags:
  - Python questions
---

`Encapsulation` - Restrict the access to methods or variables. This can prevent the data from being modified or accessing accidentally, but not intentionally.

The private attributes and methods are not really hidden, they’re renamed adding `_name` in the beginning of their name. The method can actually be called.

`Example:`

We create a class `Car` which has two methods:  `drive()` and `updateSoftware()`. When a `car` object is created, it will call the private methods `__updateSoftware()`.  

This function cannot be called on the object directly, only from within the class.

```python
class Car:

    def __init__(self):
        self.__updateSoftware()

    def drive(self):
        print('driving')

    def __updateSoftware(self):
        print('updating software')

red_car = Car()
red_car.drive()
#re_car.__updateSoftware() not accessible from object.

# Output:
updating software
driving
```

## Reference

[Encapsulation](https://pythonspot.com/encapsulation/)

[The four pillars of object orientation](https://www.freecodecamp.org/news/four-pillars-of-object-oriented-programming/)
