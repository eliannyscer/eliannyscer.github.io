---
title: "What is the difference between Python Arrays and lists?"
tags:
  - Python question
---

They are similar because an array is also a data structure that stores a collection of items. Like lists, arrays are ordered, mutable, enclosed in square brackets, and able to store non-unique items.

Arrays and lists, have `the same way of storing data`. But, arrays can hold `only a single data type` elements while lists can hold `any data type` elements.

`Example:`

```python
import array as arr
My_Array=arr.array('i',[1,2,3,4])
My_list=[1,'abc',1.20]
print(My_Array)
print(My_list)

Output:
array(‘i’, [1, 2, 3, 4]) [1, ‘abc’, 1.2]
```

## Other differences

* Arrays need to be declared is you are sing in Python.
* Arrays can store data  more efficient in special for storing large amounts of data.
* Arrays are great for numerical operations; lists cannot directly handle math operations. For example, you can divide each element of an array by the same number with just one line of code. If you try the same with a list, you'll get an error.

## Reference

[Arrays](https://learnpython.com/blog/python-array-vs-list/)
