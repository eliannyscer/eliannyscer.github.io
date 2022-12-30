---
title: "How to count the number of capital letters in a file?"
tags:
  - Python exercise
---

Your code should work even if the file is too big to fit in memory.
________________

We need to write a multiple line solution and then convert it to one liner code.

`Example:`

```python
with open(SOME_LARGE_FILE) as fh:
count = 0
text = fh.read()
for character in text:
    if character.isupper():
count += 1
```

We will now try to transform this into a single line:

```python
count sum(1 for line in fh for character in line if character.isupper())
```

## Reference

[Example](https://forums.wikitechy.com/question/write-a-one-liner-that-will-count-the-number-of-capital-letters-in-a-file-your-code-should-work-even-if-the-file-is-too-big-to-fit-in-memory/)
