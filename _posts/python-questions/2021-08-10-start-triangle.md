---
title: "How to produce a star triangle?"
tags:
  - Exercises
---

The primary purpose of creating this program is to explain the concept of the loop in the Python program in a simple example.

`Example` - Display stars in equilateral triangle:

```python
equilateral = 20
for e in range(1, 11):
    # repeat space for equilateral times
    print(" "*equilateral, end='')
    # repeat stars for e times 
    print("* "*(e))
    equilateral -= 1
```

`Output:`

```python
                    * 
                   * * 
                  * * * 
                 * * * * 
                * * * * * 
               * * * * * * 
              * * * * * * * 
             * * * * * * * * 
            * * * * * * * * * 
           * * * * * * * * * * 
```

## Additional information

You can change it to any other characters if you want. Printing a symbol works the same for any programming language. You can use the same logic on any other programming language like Java, R, C, C++,etc. to get the same output.

`Example` - Using `#` instead of `*`:

```python
equilateral = 20
for e in range(1, 11):
    # repeat space for equilateral times
    print(" "*equilateral, end='')
    # repeat hash for e times 
    print("# "*(e))
    equilateral -= 1
```

`Output:`

```python
                    # 
                   # # 
                  # # # 
                 # # # # 
                # # # # # 
               # # # # # # 
              # # # # # # # 
             # # # # # # # # 
            # # # # # # # # # 
           # # # # # # # # # # 
```

## References

[Program to create equilateral triangle](https://www.w3schools.in/python-programs/python-program-to-creating-an-equilateral-triangle-pyramid-pattern/)

[Printing triangle with different symbol](https://www.codevscolor.com/python-print-triangle-star)
