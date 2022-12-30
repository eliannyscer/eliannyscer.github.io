---
title: "How do you do data abstraction in Python?"
tags:
  - Python question
---

* Data Abstraction is providing only the required details and hiding the implementation from the world. It can be achieved in Python by using interfaces and abstract classes.

* The user is only able to view basic functionalities while the internal detail are hidden.

* To declare an Abstract class, we firstly need to import the `abc` module.

`Example:`

```python
from abc import ABC
class abs_class(ABC):
#abstract methods
```

## Additional information

People do not think of a car as a set of thousands of individual parts. Instead they see it as a well-defined object with its own unique behavior. This abstraction allows people to use a car to drive without knowing the complexity of the parts that form the car. They can ignore the details of how the engine transmission, and braking systems work. Instead, they are free to utilize the object as a whole.

The point is that we manage the complexity of the car (or any other complex system) through the use of hierarchical abstractions.

## References

[Abstraction](https://www.360digitalgyan.com/phow-do-you-do-data-abstraction-in-pythonp)

[Abstraction examples](https://www.askpython.com/python/oops/abstraction-in-python)

[The four pillars of object orientation](https://www.freecodecamp.org/news/four-pillars-of-object-oriented-programming/)
