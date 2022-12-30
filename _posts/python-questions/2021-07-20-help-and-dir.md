---
title: "What is the usage of help() and dir() function in Python?"
tags:
  - Python FAQ
---

`help() function` - It is used to display the `documentation` string and also facilitates you to see the help related to modules, keywords, attributes, etc.

`Example:`

```python
help(dict)

# Output:
Help on class dict in module builtins:

class dict(object)
 |  dict() -> new empty dictionary
 |  dict(mapping) -> new dictionary initialized from a mapping object's
 |      (key, value) pairs
 .....
```

`dir() function` - It returns all `properties` and `methods` of the specified object, without the values.

`Example:`

```python
class Person:
  name = "Ellie"
  age = 30
  country = "Spain"

print(dir(Person))

# Output:
['__class__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__module__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', '__weakref__', 'age', 'country', 'name']
```

## References

[Dir() function](https://www.w3schools.com/python/ref_func_dir.asp)

[Help() function](https://www.programiz.com/python-programming/methods/built-in/help)
