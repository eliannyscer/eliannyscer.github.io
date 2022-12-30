---
title: "How to produce a fibonacci serie in Python?"
tags:
  - Python exercise
---

`What is Fibonacci Series?` - It is a series of numbers formed by the sum of the two preceding numbers in the series.

```python
 0,1,1,2,3,5
```

* The `1` is found by sum the two numbers before it (0+1)

* The `2` is found by sum the two numbers before it (1+1)

* The `3` is found by sum the two numbers before it (2+1)

* The `5` is found by sum the two numbers before it (2+3)

`It is done until the number of terms you want or requested by the user`.

`Example:`

```python
length = int(input("Enter length: "))
#first element of series
first_element = 0  
#second element of series                                      
second_element=1                                       
if length<=0:
    print("The requested series is",first_element)
else:
    print(first_element,second_element,end=" ")
    for x in range(2,length):
        next=first_element+second_element                           
        print(next,end=" ")
        first_element = second_element
        second_element = next
```

`Output` - Using the number 8 as input:

```text
0 1 1 2 3 5 8 13
```

Using a negative number the requested series is `0`.

## References

[What is Fibonacci Series?](https://www.edureka.co/blog/python-fibonacci-series/)

[Fibonacci series explanation](https://www.pythonpool.com/fibonacci-series-in-python/)
