---
title: "How is memory managed in Python?"
tags:
  - Python questions
---

1. Memory management in python is managed by Python private space. All objects and data structures are located in a private place. The programmer does not have access, the python interpreter takes care of this instead.

2. The object allocation and de-allocation is done by Python’s memory manager,the process is automatic but the programmer have access to some tools to code.

3. Python has an garbage collector to recycle all the unused memory to make it available for other objects.

`Example (Memory is an empty book)`

You can begin by thinking of a computer’s memory as an empty book for short stories. There’s nothing written on the pages yet. Eventually, `different authors` will come. Each author wants some space to write their story in the book.

Since `they aren’t allowed to write over each other`, they must be careful about in which pages they write. Before they begin writing, `they consult the manager` of the book. The manager then `decides` where in the book they’re allowed to write.

When no one reads or references the stories, they are `removed` for somebody to make space for new stories.

`The authors` are like `different applications` or processes that need to store data in memory. `The manager`, who decides where the authors can write in the book, plays the role of a `memory manager` . The person `who removed` the old stories to make room for new ones is a `garbage collector`.

Additionally you can thing in the `reference` like the number of the page in the book where you can find the story (the reference is the address where you can to locate the story).

## Additional information

Python uses `two` strategies for memory allocation:

1. `Garbage collection` - python has an garbage collector to recycle all the unused memory and make it available for other objects.

2. `Reference counting` - it's the number of references that you have. A  reference is a name, it work as container object pointing at another object.

### How we can increase the reference counter?

* This increase the number of reference by 1:

```python
E = 26

# E ----> +1 reference (26)
# Reference count: 1
```

* Instead of create a need slice in the memory, it just adding other reference and now the reference count is 2:

```python+
E = 26
K = 26

# E ----> +1 reference (26)
# K ----> +1 reference (26)
# Reference count: 2
```

* It will continue increase if the reference is always the same:

```python+
Z = [26, 26]

# Z ----> +2 reference (26 - 26)
# Reference count: 4
```

## Why should you care the memory managed ?

Knowing about memory management helps you write more efficient code.

## How are python objects stored in memory?

Name --> References --> Objects

A `name` is just a label for an object and each object can have lots of names and those names reference that objects. A reference is a name or a container object pointing at another object.

### Different types of objects

* Simple (eg.number or strings)
* Containers ( eg.dictionary, list or classes)

References:

[Memory Management in Python-The Basics-PyCon-2016](https://www.youtube.com/watch?v=F6u5rhUQ6dU&t=429s)
[Garbage collection and reference counting](https://www.geeksforgeeks.org/memory-management-in-python/)
[How is the memory managed](https://www.i2tutorials.com/how-is-memory-managed-in-python/)
[Memory as a empty book](https://realpython.com/python-memory-management/ç)
[Garbage collection](https://www.geeksforgeeks.org/garbage-collection-python)
