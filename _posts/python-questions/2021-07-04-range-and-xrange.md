---
title: "What is the difference between range and xrange?"
tags:
  - Python FAQ
---

The principal difference is that `range` returns a Python `list` object and `xrange` returns an `xrange` object.

This means that xrange doesn’t actually generate a static list at run-time like range does. It creates the values as you need them with a special technique called yielding.

## Additional information

In Python `2`  there was both methods to generate a list of integers. In Python `3`, there is no `xrange`, the `range()` function in python `3` is just a re-implementation of the `xrange()` of python `2`.

In terms of functionality `xrange` and `range` are the exact same.

## Other different

* `Memory consumption` - The `range()` function takes more memory that use the `xrange()` function. The basic reason for this is the return type of `range()` is `list` and `xrange()` is `xrange()`.
  
* `Speed` - xrange is faster than the standard range function because this function only evaluates like a lazy evaluation, therefore is faster in implementation than `range()`.

## References

[Range vs. xrange](https://www.geeksforgeeks.org/range-vs-xrange-python/)

[Differences between range and xrange](https://www.techbeamers.com/python-xrange-range/)

[Definition](https://getpocket.com/read/1965283225)
