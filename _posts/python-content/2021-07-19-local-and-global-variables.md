---
title: "What are local variables and global variables in Python?"
tags:
  - Python FAQ
---

## Global variable

It is defined and declared outside a function and we need to use them inside a function. These variables can be accessed by any function in the program.

`Example:`

```python
def function():
    print(g_variable)

g_variable = "You are using a global variable!"
function()

# Output:
You are using a global variable!
```

The variable `g_variable` is defined as the string “You are using a global variable!” before we call the function `function()`. The only statement in `function()` is the `print s` statement. As there are no locals, the value from the globals will be used.

`Other example:`

If a variable with the same name is defined inside of the function  then it will print the value given inside the function only and not the global value.

```python
def function():
    g_variable = "I am new variable inside the function!"
    print(g_variable)
    
g_variable = "You are using a global variable!"

function()

# Output:
I am new variable inside the function!
```

`Example with an error:`

We have this error because we print the function before define the variable.

```python
def function():
    print(l_variable)
    l_variable = "This is a local variable!"
 
g_variable = "This sis a global_variable!"
function()
print(g_variable)

# Output:
UnboundLocalError: local variable 'l_variable' referenced before assignment
```

To tell Python, that we want to use the global variable, we have to use the keyword `global`.

`Example:`

```python
def function():
    global g_variable
    print(g_variable)
    local_variable = "This is a local variable!"
    print(local_variable)
 
# "g" for global
g_variable = "This is a global variable!"
function()

# Output:
This is a global variable!
This is a local variable!
```

* Local Variable:

Any variable declared inside a function is known as a local variable. This variable is present in the local space and not in the global space.

```python
def calculation():
    local_variable = 10
    local_variable = local_variable * 10
    print(local_variable)
calculation()

# Output:
100
```

`Note:` A local variable can't access to a global variable.

## Reference

[Global and local variables](https://www.geeksforgeeks.org/global-local-variables-python/)