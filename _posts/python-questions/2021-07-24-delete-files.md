---
title: "How can files be deleted in Python?"
tags:
  - Python questions
---

To delete a file, you must import the `os` module, and run the `os.remove()` function:

```python
import os
os.remove("practice.py") 
```

After this you will see next to the tittle of your file the word `deleted`, if you check in the original folder you will see that the file doesn't exist.

```text
practice.py(deleted)
```

## Reference

[Delete file](https://www.w3schools.com/python/python_file_remove.asp)