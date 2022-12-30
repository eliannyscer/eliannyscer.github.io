---
title: "What does an object() do?"
tags:
  - Python questions
---

* The `object()` function returns an empty object.

* You cannot add new properties or methods to this object.

* This object is the base for all classes, it holds the built-in properties and methods which are default for all classes.
  
`Example:`

```python
test = object()

print(type(test))
print(dir(test))
```

`Output:`

```python
<class 'object'>
['__class__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__']
```

## Additional information

An object is a fundamental building block of an object-oriented language. Integers, strings, floating point numbers, even arrays and dictionaries, are all objects. More specifically, any single integer or any single string is an object. The number 12 is an object, the string "hello, world" is an object, a list is an object that can hold other objects, and so on. You've been using objects all along and may not even realize it.

## References

[Definition and Usage](https://www.w3schools.com/python/ref_func_object.asp)

[Object() examples](https://www.programiz.com/python-programming/methods/built-in/object)

[What is an object?](https://stackoverflow.com/questions/56310092/what-is-an-object-in-python)
