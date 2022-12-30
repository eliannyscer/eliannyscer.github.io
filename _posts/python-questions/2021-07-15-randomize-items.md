---
title: "How can you randomize the items of a list in place in Python?"
tags:
  - Python questions
---

The random module provides a `shuffle()` function that returns a sequence with its elements randomly.

`Example:`

```python
import random
numbers = [1, 2, 3, 4, 5, 6,]
random.shuffle(numbers)
print(numbers)

# Output:
[4, 3, 6, 1, 5, 2]
```

## Reference

[Example and definition](https://www.tutorialspoint.com/How-to-randomize-the-items-of-a-list-in-Python)
