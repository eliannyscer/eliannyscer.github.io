---
title: "What are docstrings in Python?"
tags:
  - Python question
---

* Python documentation strings (or docstrings). It is used like a comment, to `document` a specific segment of code.

* The docstring should describe `what the function does`, not how.

* It must be `the first statement` in the object’s definition.
  
* It begins with a `capital letter` and ends with a `period`.

* They are declared using '''triple `single` quotes''' or """triple `double` quotes""".

`Example:`

```python
def decrement(number):
    """This is the docstring of this function.
    
    It describes what the function does, what are its calling conventions and
        what are its side effects"""
    number=number-1
    return number
```

## Additional information

## Comments vs. docstrings

Both are written using multiline strings but they are not completely same:

`Comment` - This are used to increase the understandability of the code and they generally explain why a statement has been used in the program.

`Docstring` -This are used to associate the documentation with the objects like classes, methods and functions in python and they describe what the object does.

## References

[Docstrings](https://www.geeksforgeeks.org/python-docstrings/)

[Comments vs. docstrings - examples](https://www.pythonforbeginners.com/comments/difference-between-comments-and-docstrings-in-python)
