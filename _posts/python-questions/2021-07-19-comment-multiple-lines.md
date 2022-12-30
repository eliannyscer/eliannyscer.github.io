---
title: "How to comment multiple lines in python?"
tags:
  - Python question
---

Python does not really have a syntax for multi line comments. To add a multiline comment you could insert a `#` for each line.

`Example:`

```python
#This is a comment
#written in
#more than just one line
print("Hello, World!")

# Output:
Hello, World!
```

Other way to do it is adding a multi-line string (triple quotes or three single quotes) in your code, and place your comment inside it, you can do it because python ignore string that are not assigned to a variable.

`Example:`

```python
"""
This is a comment
written in
more than just one line
"""
print("Hello, World!")

# Output:
Hello, World!
```

## References

[Multiple lines comments](https://www.w3schools.com/python/gloss_python_multi_line_comments.asp)

[Shortcut to comment out multiple lines](https://stackoverflow.com/questions/6173118/shortcut-to-comment-out-multiple-lines-with-python-tools-for-visual-studio)
