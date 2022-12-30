---
title: "What are the generators in python?"
tags:
  - Python questions
---

It is Functions that return iterable items to do it use the `yield keyword` instead than `return`. If the body of a `def` function contains `yield`, the function automatically becomes a generator function.

```Python
def simple_generator():
    yield 1            
    yield 2            
    yield 3            
   
# Code to check the generator function
for value in simple_generator(): 
    print(value)

# Output:
1
2
3
```

## Reference

[Generators in python](https://www.geeksforgeeks.org/generators-in-python/)
