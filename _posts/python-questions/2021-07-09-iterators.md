---
title: "What are python iterators?"
tags:
  - Python questions
---

* An `iterable` is any object that can return an iterator and an `iterator` is the object used to iterate over an iterable object.

* This implements __iter__ and __next__ methods.

* This can interact with iterable objects like lists, tuples, dicts, and sets. An object which will return data, one element at a time.

`Example:`

```python
my_obj = {"Python", "Iterator"}
iter_obj = iter(my_obj)
print(next(iter_obj))

# Output:
Iterator
```

## Additional information

## Iterator protocol

`__iter__` - This method  is called for the initialization of an iterator. This returns an iterator object.

`__next__` - This next method returns the next value for the iterable.

## References

[Iterator](https://www.pythontutorial.net/advanced-python/python-iterators/)

[Example](https://www.edureka.co/blog/python-iterator)

[Definition](https://blog.avenuecode.com/containers-iterables-iterators-and-generators)

[Iterators basics](https://www.geeksforgeeks.org/iterators-in-python/)

[Python Iterator](https://www.programiz.com/python-programming/iterator)
