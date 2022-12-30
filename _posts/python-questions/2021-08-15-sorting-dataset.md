---
title: "How to sort an algorithm for a numerical dataset?"
tags:
  - exercises
---

The Python language, like many other high-level programming languages, offers the ability to sort data out of the box using `sort()`. You can use to sort any list as long as the values inside are comparable.

`Example:`

```python
list = ["1", "9", "0", "9", "5"]
list = [int(i) for i in list]
list.sort()
print (list)

# Output:
[0, 1, 5, 9, 9]
```

## Additional information

`sort()` is a method of list class and can only be used with lists.

## References

[Sort() and sorted()](https://realpython.com/python-sort/#ordering-values-with-sort)

[Sorting Data With Python - Course](https://realpython.com/courses/python-sorting-data/)

[Different kinds of sorting algorithm](https://realpython.com/sorting-algorithms-python/#the-importance-of-sorting-algorithms-in-python)

[Difference between sorted() and sort()](https://www.geeksforgeeks.org/python-difference-between-sorted-and-sort/)
