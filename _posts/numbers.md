# Python Numbers

There are three numeric types in Python. Variables of numeric types are created when you assign a value to them:

## int

Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.

`Example:`

```python
e = 2
l = 19958336363838373
i = -584783093049

print(type(e))
print(type(l))
print(type(i)) 
```

`Output:`

```text
<class 'int'>
<class 'int'>
<class 'int'>
```

## Integer division

- Integer division produces a floating point result
- This was different in python 2

`Example:`

```python
print (8/2)
print (7/2)
print(99/100)
print (6.1/ 1.0)
```

`Output:` As a result you can see that everyone have decimal, even if is a whole number

```python
4.0
3.5
0.99
6.1
```

## float

Float, or "floating point number" is a number, positive or negative, containing one or more decimals.

`Example:`

```python
e = 2.6
l = 1.60
i = -26.86

print(type(e))
print(type(l))
print(type(i)) 
```

`Output`:

```txt
<class 'float'>
<class 'float'>
<class 'float'>
```

`Note: It's important to use a comma because if you use a comma the type will be other (tuple).`

Example:

```python
e = 2,6
print(type(e))

#Output
<class 'tuple'>
```

## complex

Complex numbers are used in many applications related to mathematics. For example, an electric circuit which is defined by voltage(V) and scientific calculations and others calculus and python provides useful tools to manipulate them.

`Example:`

```python
e = 2 + 6j
l = 2j
i = -6J
print(type(e))
print(type(l))
print(type(i))
```

`Output`:

```txt
<class 'complex'>
<class 'complex'>
<class 'complex'>
```

In Electronics ‘i’ is used to represent current and hence they use ‘j’ to represent iota. Python adheres to this same convention.

## Type Conversion

You can convert from one type to another with the int(), float(), and complex() methods.

`Example` - Convert from int to float:

```python
e = 2
a = float(e)
print(a)
print(type(a))

#Output
2.0
<class 'float'>
```

`Example` - Convert from float to int:

```python
l = 2.6
b = int(l)
print(b)
print(type(b))

#Output
2
<class 'int'>
```

`Example` - Convert from int to complex:

```python
e = 2
c = complex(e)
print(c)
print(type(c))

#Output
(2+0j)
<class 'complex'>
```

`Note: You cannot convert complex numbers into another number type.`

## String conversion

- You can also use `int()` and `float()` to convert between strings and integers
- You will get an error if the string does not contain numeric characters

`Example:` If you try to mix a string with a integer you will have a error:

```python
number = "123"
print(number + 1)

#Output
print(number + 1)
TypeError: can only concatenate str (not "int") to str
```

But you can convert a string in integer without problem if this contains numbers:

```python
number = "123"
print(type(number))
number1 = int(number)
print(type (number))
print(number1 + 1)

#Output

<class 'str'>
<class 'str'>
124
```

## Random number

Can be used to make random numbers. Import the random module, and display a random number between  the number that you define.
The random module has several methods, for this example i will show 2 with the result:

randrange /randint= Returns a random number between the given range.

`Example:`

```python
import random
print(random.randint(0, 100)) 

#Output 
80
```
