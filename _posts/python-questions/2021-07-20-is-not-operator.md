---
title: "What is the purpose of is not and in operators?"
tags:
  - Python questions
---

Operators are special functions. They take one or more values and produce a corresponding result.

`is` - It is used to check if two values (or variables) are located on the same part of the memory. It returns `True` when 2 operands are `True` or `False` is they are not equal.

`Example:`

```python
a = 1 
b = 3
print( a is b)

# Output:
False
```

`not` -  This will return  `True` if the statement(s) is not `True`, otherwise it will return `False` (returns the inverse of the boolean value).

`Example:`

```python
x = False
print(not x) 

# Output:
True
```

`in` - This checks if some element is present in some sequence.

`Example:`

```python
fruits = ["Apple", "Banana", "Cherry"]
print("Coconut" in fruits)

# Output:
False
```

## References

[Python operators](https://www.programiz.com/python-programming/operators)

[Not operator - Example](https://www.w3schools.com/python/ref_keyword_not.asp)
