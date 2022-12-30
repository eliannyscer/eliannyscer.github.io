---
title: "How to remove values to a python array?"
tags:
  - Python FAQ
---

Array elements (list) can be removed using `pop()` or `remove()` method. The difference between these two functions is that the first one returns the deleted value and work with the index while the second does not returns the deleted value and work with the name of the item.

## Using remove()

It takes a single element as an argument and removes it from the list.

`Example:`

```python
list = [ "Hello", "Labas", "Hallo", "Hola"]
list.remove("Hello")
print(list)

#Output:
['Labas', 'Hallo', 'Hola']
```

## Using pop()

We can remove the element at the specified index and get the value of that element using pop().

`Example` - Delete a value using index:

```python
list = [ "Hello", "Labukas", "Hallo", "Hola"]
list.pop(2)
print(list)

# Output:
['Hello', 'Labukas', 'Hola']
```

`Example` - Return the deleted value:

```python
list = [ "Hello", "Labas", "Hallo", "Hola"]
list.pop(2)
print(list)
print(list.pop(2))

# Output:
['Hello', 'Labas', 'Hola']
Hola
```

## Additional information

### Using del

The `del´ statement is not a function of List but is working like pop. Items of the list can be deleted using del statement by specifying the index of item (element) to be deleted.

```python
list = [ "Hello", "Labas", "Hallo", "Hola"]
del list[1]
print(list)

# Output:
['Hello', 'Hallo', 'Hola']
```

## References

[Examples](https://www.geeksforgeeks.org/how-to-remove-an-item-from-the-list-in-python/)

[Remove()](https://www.programiz.com/python-programming/methods/list/remove)