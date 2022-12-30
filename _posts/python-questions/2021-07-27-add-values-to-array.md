---
title: "How to add values to a python array?"
tags:
  - Python question
---

## Append

`Syntax` - `list.insert(element)`.

With this method, you can add a single element `to the end` of a list.

`Example` - Append a integer:

```python
numbers = [1, 2, 3, 4]
numbers.append (8)
print(numbers)

# Output:
[1, 2, 3, 4, 8]
```

## Insert

`Syntax` - list.insert(position, element).

This method is used to insert an element `at a particular index` (position) in the list.

`Example` - Insert a string:

```python
letters = ["a", "b", "c", "d"]
letters.insert(2, "Z")
print(letters)

# Output:
['a', 'b', 'Z', 'c', 'd']
```

## Extend

`Syntax` - list.extend(list elements).

This method adds a `specified list elements` (or any iterable) to the end of the current list.

`Example` - Extend a dictionary

```python
consonants = [{"b": 1, "c": 2, "d": 3, "f": 5}]
vowels = [{"a": 0, "e": 4, "i": 6}]
consonants.extend(vowels)
print(consonants)

# Output:
[{'b': 1, 'c': 2, 'd': 3, 'f': 5}, {'a': 0, 'e': 4, 'i': 6}]
```

## References

[List append and insert](https://www.freecodecamp.org/news/python-list-append-how-to-add-an-element-to-an-array-explained-with-examples/)

[List extend](https://www.w3schools.com/python/ref_list_insert.asp)

[Examples](https://www.freecodecamp.org/news/python-list-append-how-to-add-an-element-to-an-array-explained-with-examples/)
