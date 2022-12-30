---
title: "What does [::-1] do?"
tags:
  - Python question
---
It means that for a given string/list/tuple, you can slice the said object using the format:

`<object_name>[<start_index>, <stop_index>, <step>]`

`Example:`

```python
a = "1-2-3-4-5-6"
print (a[::-1])

# Output:
6-5-4-3-2-1
```

## Additional information

The object is going to slice every "step" index from the given start index, till the stop index (excluding the stop index) and return it to you.

In case the start index or stop index is missing, it takes up the default value as the start index and stop index of the given string/list/tuple. If the step is left blank, then it takes the default value of 1 i.e it goes through each index.

## References

[Definition](https://stackoverflow.com/questions/31633635/what-is-the-meaning-of-inta-1-in-python)

[Link](https://stackoverflow.com/questions/28535392/what-does-n-1-means-in-python)
