---
title: "Is indentation required in python?"
tags:
  - Python question
---

Yes, it is necessary because specifies a block of code. It is a way of telling a Python interpreter that a group of statements belongs to a particular block of code.

`Example:`

You are reading a book without the page numbers and you are  missing because you don't know  where to continue reading and you will get confused. This situation is similar with Python. Without indentation, Python does not know which statement to execute next or which statement belongs to which block. This will show a IndentationError.

## Additional information

## Indentation

In simple terms indentation refers to adding white space before a statement. because indentation refers to the spaces at the beginning of a code line and specify a block of code.

Example:

You need to use the indentation with the print function

```python3
if 10 > 5:
  print("Ten is greater than five!")

#Output:
ten is greater than five!
```

Otherwise you will have an error, because you skipped the indentation:

```python3
if 10 > 5:
print("Ten is greater than five!")

#Output:
IndentationError: expected an indented block
```

## Interesting fact

* Most of the programming languages like C, C++, Java use braces { } to define a block of code, python uses indentation.

* Python uses 4 spaces as indentation by default. However, the number of spaces is up to you, but a minimum of 1 space has to be used.

## References

[Indentation definition](https://www.w3schools.com/python/gloss_python_indentation.asp)

[Indentation example](https://www.geeksforgeeks.org/indentation-in-python/)
