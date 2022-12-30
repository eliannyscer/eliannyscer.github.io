---
title: "How to import modules in python?"
tags:
  - Python questions
---

Python modules can get access to code from another module by importing the file/function using the keyword `import`. You can do it in different  ways:

* `Example` - Using the original module name:

* Syntax - `import` [module]

```python
import random
print(random.randint(0, 5))

# Output - Alt number:
3
```

* `Example` - Import a specific function from a specific module:

* Syntax - `from` [module] `import`[function].

```python
from random import randint
print(randint(0, 5))

# Output - Alt number:
2
```

* `Example`- Using an alias name

* Syntax - `import` [module] `as` [alias]

```python
import random as r
print(r.randint(0, 5))

# Output - Alt number:
5
```

* `Example` - imports everything present in the module:
  
* Syntax - `from` [module] `import` *

```python
from random import *
print(randint(0, 5))

# Output - Alt number:
44
```

## Reference

[Import module - Examples](https://www.wikihow.com/Import-a-Module-Into-Python)