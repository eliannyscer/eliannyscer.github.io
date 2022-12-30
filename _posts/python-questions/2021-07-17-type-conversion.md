---
title: "What is type conversion in Python?"
tags:
  - Python questions
---

It convert one data type to another.

## Additional information

There are two types of Type Conversion in Python:

* `Implicit Type Conversion` - The Python interpreter automatically converts one data type to another.

`Example:`

```python
E = 30
print("E = ",type(E))
K = 33.0
print("K = ",type(K))
E = E + K
print("E = ", E)
print('Now "E" have different type!',type(E))

Output:
E =  <class 'int'>
K =  <class 'float'>
E =  63.0
Now "E" have different type! <class 'float'>
```

You can see the type 'E' is automatically changed to the “float” type from the “integer” type. This is a simple case of Implicit type conversion in python.

* `Explicit Type Conversion` - The data type is manually changed by the user.

## Data type examples

`int()` – converts any data type into integer type

```python
E = 30
print(float(E))

#Output:
30.0
```

`float()` – converts any data type into float type

```python
K = 33.6
print(int(K))

#Output:
33
```

`ord()` – converts characters into integer

```python
character_to_integer = ord("E")
print ("After converting character to integer: ", character_to_integer)

#Output:
After converting character to integer: 69
```

`hex()` – converts integers to hexadecimal

```python
int_to_hex = hex(30)
print ("After converting 30 to hexadecimal string : ", int_to_hex)

#Output:
After converting 30 to hexadecimal string : 0x1e
```

`oct()` – converts integer to octal

```python
int_to_oct = oct(33)
print ("After converting 33 to octal string : ", int_to_oct)

#Output:
After converting 33 to octal string :  0o41
```

`tuple()` – This function is used to convert to a tuple.

```python
E = "Ellie"
K = tuple(E)
print ("After converting string to tuple:", K)

#Output:
('E', 'l', 'l', 'i', 'e')
```

`set()` – This function returns the type after converting to set.

```python
E = "Ellie"
K = set(E)
print ("After converting string to set : ", K)

#Output:
After converting string to set :  {'l', 'E', 'i', 'e'}
```

`list()` – This function is used to convert any data type to a list type.

```python
E = "Ellie"
K = list(E)
print ("After converting string to list : ", K)

#Output:
After converting string to list :  ['E', 'l', 'l', 'i', 'e']
```

`dict()` – This function is used to convert a tuple of order (key,value) into a dictionary.

```python
tup = (('a', 1) ,('f', 2), ('g', 3))
c = dict(tup)
print ("After converting tuple to dictionary: ", c)

#Output:
After converting tuple to dictionary: {'a': 1, 'f': 2, 'g': 3}
```

`str()` – Used to convert integer into a string.

```python
a = 1
c = str(a)
print ("After converting integer to string: ", c)

#Output:
After converting integer to string: 1
```

`complex(real,image)` – This function converts real numbers to complex(real) number.

```python
c = complex(1,2)
print ("After converting integer to complex number : ", c)

#Output:
After converting integer to complex number :  (1+2j)
```

## References

[Data types](https://www.geeksforgeeks.org/type-conversion-python/)

[Code examples](https://www.geeksforgeeks.org/type-conversion-python/)