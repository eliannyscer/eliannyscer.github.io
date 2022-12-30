---
title: "What are negative indexes and why are they used?"
tags:
  - Python questions
---

Python programming language `supports negative indexing of arrays(list)`, something which is not available in arrays in most other programming languages.

This means that the index value of `-1` gives the last element, and `-2` gives the second last element of an array. The negative indexing starts from where the array ends.

This means that the last element of the array is the first element in the negative indexing which is -1.

`Example` - Normal index

```python
list = [10, 20, 30, 40]
print(list[2])

# Output:
30
```

`Example:`

```python
list = [10, 20, 30, 40]
print(list[-1])
print(list[-3])

# Output:
40
20
```

## References

[Negative index](https://brainly.in/question/9668383)

[Example](https://www.i2tutorials.com/what-are-negative-indexes-and-why-are-they-used/)
