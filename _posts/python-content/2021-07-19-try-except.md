---
title: "Python Try Except"
categories:
- Programming
tags:
- Python
---

{% include video id="j2kTcc1lcK8" provider="youtube" %}

- With the `try` function you can test a block of code for errors.

- The `except` block allow you handle or manipulate the error.

- The `finally` block lets you execute code, regardless of the result of the try- and except blocks.

## Try

When an error occurs, or exception as we call it, Python will normally stop and generate an error message.These exceptions can be handled using the try statement:

The try block will generate an exception, because `e` is not defined,

`Example:`

```python
try:
  print(e)
except:
  print("An exception occurred") 

# Output:
An exception occurred
```

`Since the try block raises an error, the except block will be executed. Without the try block, the program will crash and raise an error:`

```python
print(e)

# Output:
NameError: name 'e' is not defined
```

## Some Exceptions

You can define as many exception blocks as you want,  if you want to execute a special block of code for a special kind of error.

`For example you can print one message if the try block raises a NameError and another for other errors:`

Example:

```python
try:
  print(e)
except NameError:
  print('You need to define the variable "e" ')
except:
  print("Something else went wrong") 

# Output:
You need to define the variable "e"
```

## Else

The else clause is executed if and only if no exception is raised. This is different from the finally clause that’s always executed.

`Example:`

```python
try:
    e = "Hello"
except:
    print('"e" is not definite')
else:
    print('No exception occurred')

# Output:
No exception occurred
```

## Else with many exceptions

You can catch many types of exceptions in this way, but remember that `the else clause` is executed `only` if no exception happens.

`Example:`

```python
try:
    e = "Hello"
except NameError:
    print('"e" was not defined')
except ValueError:
    print(' A value error ocurred')
except TypeError:
    print( 'A TypeError ocurred')
else:
    print('No exception occurred')
finally:
    print("It's all")
```

`Output:`

```txt
No exception occurred
It's all
```

## Finally

A try-except block can have the finally clause (optionally). The finally clause is always executed.
So the general idea is this.

`Example:`

```python
try:
    e = "Hello"
except:
    print('"e" is not definite')
else:
    print('No exception occurred')
finally:
    print("It's all")
```

`Output:`

```txt
No exception occurred
It's all
```

## Raise Exception

-Exceptions are raised when an error occurs. But in Python you can also `force an exception` to occur with the keyword `raise`.
-You can define what kind of error to raise, and the text to print to the user.

Any type of exception can be raised.

`Example:`

```python
number = "1.0"
if type(number) is not int:
  raise TypeError("Only integers are allowed")

# Output:
TypeError: Only integers are allowed
```

`Example` - Raise an error and stop the program if e is lower than 50:

```python
e = 26
if e < 50:
  raise Exception("Sorry, you cannot continue!")

# Output:
Exception: Sorry, you cannot continue!
```
