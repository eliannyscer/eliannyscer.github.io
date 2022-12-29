---
title: "Boolean Values"
tags:
  - Python
---

Is a data type that has one of two possible values (usually denoted true and false).

{% include video id="_Bi7i7kyTuM" provider="youtube" %}

In programming you often need to know if an expression is `True` or `False`.
When you compare two values, there is only two possible answers,
the expression is evaluated and Python returns the Boolean answer:

`Example:`

```Python
print(2 == 6)
print ( 9 > 7)
print(2 < 6)

#Output:
False
True
True
```

When you run a condition in an if statement, Python returns True or False

`Example:`

```python
e = 995
c = 26

if c > e:
  print("c is greater than e!")
else:
  print("c is not greater than e!")

# Output:
c is not greater than e!
```

## Type

 You can check the type of True and False with the built-in type():

`Example:`

```python
type(False)
<class 'bool'>

type(True)
<class 'bool'>
```

## Python Booleans as Keywords

It’s possible to assign a Boolean value to variables, but it’s not possible to assign a value to True.

`Example:`

```python
True_1= True
print(True_1)
#Output:
True
```

```python
True = 5 
#Output:
SyntaxError: cannot assign to True
```

The same rule applies to False:

```python
False_1= True
print(False_1)

#Output:
True
```

```python
False = 26
print(False)

#Output:
SyntaxError: cannot assign to False

```

## Evaluate two variables

The bool() function allows you to evaluate any value, and give you True or False in return.

`Example:`

```python
e = "Hello"
l = 27
i = -1

print(bool(e))
print(bool(l))
print(bool(i))

#Output:
True
True
True
```

## Most Values are True

Almost any value is evaluated to True if it has some kind of content:

- Any string is True, except `empty strings`.

- Any number is True, except `0`.

- Any list, tuple, set, and dictionary are True, except `empty ones`.

## Some Values are False

In fact, there are not many values that evaluate to False, except empty values, such as `(), [], {}, ""`, the number `0`, and the value None. And of course the value `False` evaluates to False.

- bool(False)
- bool(None)
- bool(0)
- bool("")
- bool(())
- bool([])
- bool({})

`Example:`

```python
e = (0)
print(bool(e))

#Output:
False
```

## Functions can Return a Boolean

You can create functions that returns a Boolean Value.

`Example:`

```python
def myFunction() :
  return False

print(myFunction()) 

#Output:
False
```
