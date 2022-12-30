---
title: "How can you generate random numbers in Python?"
tags:
  - Python question
---

Random module is the standard module that is used to generate a random numbers.

* The function `random.random()` is a absolute basic random number generation.

* The function random() returns the next random float in the range [0.0, 1.0].
  
* To use the `random()` function, call the `random()` method to generate a real (float) number between 0 and 1.

`Example:`

```python
import random
x = random.random()
print(x) 

# Output:
0.4218281360071646
```

## Additional Information

The function `random()`  generates a number between 0 and 1. But there are other like the functions `randint`(min,max) and `randrange`(max), this can generated randoms numbers too but in a different way.

## Reference

[Random numbers](https://pythonprogramminglanguage.com/randon-numbers/)
