---
title: "What is a Bubble sort algorithm?"
tags:
  - exercises
---

`Bubble sort`

The basic idea is that a given list or sequence of data is verified for the order of neighboring elements by comparing them with each other. Elements are swapped if the order does not match the expected result. For example, if the expected result is a sorted list in the ascending order, once the comparison is performed, if the first element is greater than the second, they are swapped.

`Example:`

```python
def bubble_sort(numbers):
    n = len(numbers)

    for k in range(n - 1):
        flag = 0

        for e in range(n - 1):
            
            if numbers[e] > numbers[e + 1] : 
                tmp = numbers[e]
                numbers[e] = numbers[e + 1]
                numbers[e + 1] = tmp
                flag = 1

        if flag == 0:
            break

    return numbers

numbers_list= [30,7,9,33,1] 

result = bubble_sort(numbers_list)

print (result)
```

`Output:`

```python
[1, 7, 9, 30, 33]
```

## References

[Bubble sort explanation](https://nickmccullum.com/python-bubble-sort-algorithm/)

[Bubble sort example](https://www.guru99.com/bubble-sort.html)
