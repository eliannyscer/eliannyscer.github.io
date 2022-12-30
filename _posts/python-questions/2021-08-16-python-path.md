---
title: "What is PYTHONPATH?"
tags:
  - Python question
---

It is an environment variable which is used when a module is imported (allow users to import modules that have not been installed yet), you can configure to add additional directories where python will look for modules and packages.
For most installations, you should not configure these variables since they are not needed for Python to run. Python knows where to find its standard library.

## Additional information

`Example:`

You define a module:

```python
def module_func():
    print("You just imported the module)
```

Now if you try to import `the_my_module.py` you will have the following error:

```python
#Import the module
import my_module

#Call the module function
my_module.module_func()

#Output
ModuleNotFoundError: No module named 'my_module'
```

The Python interpreter cannot find the location of my_module.py file. You need to set PYTHONPATH.

## Environment variable

The environment variables influence Python’s behavior and Provide a great way to configure your Python application

References:

[Pythonpath definition](https://www.tutorialspoint.com/What-is-PYTHONPATH-environment-variable-in-Python)

[Pythonpath example](https://www.geeksforgeeks.org/pythonpath-environment-variable-in-python/)
