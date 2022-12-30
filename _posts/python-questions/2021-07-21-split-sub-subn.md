---
title: "Explain split(), sub(), subn() methods of “re” module in Python"
tags:
  - Python question
---

## Regular expression

A Regular Expression or (RegEX) is a stream of characters that forms a pattern.
Whether a string contains this pattern or not can be detected with the help of regular expressions.
It’s very easy to create and use Regular Expressions in Python - by importing `re` module.

```python
import re
```

## split()

This function splits the string. It should be imported before using it in the program.

`Example-1:`

```python
from re import split
print(split("\W+", "Words, words , Words"))

# Output:
['Words', 'words', 'Words']
```

`Example-2:` - Error

```python
from re import split
# If you don't use this "\W+" 
# you will have a error 
# because is part of the function
print(split("Words, words , Words"))

# Output:
TypeError: split() missing 1 required positional argument: 'string'
```

## Sub()

This function find all the substring where  a certain regular expression matches and then replace them with a different string.

`Syntax`: - `re.sub(pattern, repl, string, count=0, flags=0)`. `count` and `flags` are optionals.

```python
import re

pattern = "[0-9]+"
repl = "NN"
string = "Account Number - 12345, Amount - 586.32"

print("Original string:")
print(string)

result = re.sub(pattern, repl, string)

print("After replacing:")
print(result)
```

```text
# Output:

Original string:
Account Number - 12345, Amount - 586.32
After replacing:
Account Number - NN, Amount - NN.NN
```

## subn()

This function is similar to `sub()` but the output is different. It returns a tuple with count of total of all the replacements.

```python
import re

def add(m):
    # Convert.
    v = int(m.group(0))
    # Add 2.
    return str(v + 1)

# Call re.subn.
result = re.subn("\d+", add, "1 2 3 4 5")

print("Result string:", result[0])
print("Number of substitutions:", result[1])

Output

Result string: 11 21 31 41 51
Number of substitutions: 5
```

## References

[Official python documentation](https://docs.python.org/3/library/re.html?highlight=sub#re.sub)

[Sub-Example](https://pythonexamples.org/python-re-sub/)

[Subn](https://www.quora.com/What-are-split-sub-and-subn-methods-in-Python?share=1)

[Regular expression](https://www.codespeedy.com/re-sub-in-python/)
