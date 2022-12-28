# Tuple

- This are used to store multiple items in a single variable.

- It is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage.

- It is a collection which is ordered and unchangeable.

- This are written with round brackets.

`Example:`

```python
numbers = ("One", "Two", "Three")
print(numbers)

# Output:
('One', 'Two', 'Three')
```

## Tuple Items

Tuple items are ordered, unchangeable, and allow duplicate values.

- `Indexed:` the first item has index [0], the second item has index [1] etc.
  
- `Ordered:` When we say that tuples are ordered, it means that the items have a defined order, and that order will not change.

- `Unchangeable:` This means that we cannot change, add or remove items after the tuple has been created.

- `Allow Duplicates:`  Since tuple are indexed, tuples can have items with the same value.

`Example:`

```python
numbers = ("One", "Two", "Three", "Two", "Three")
print(numbers)

# Output:
('One', 'Two', 'Three', 'Two', 'Three')
```

## Length

To determine how many items a tuple have, use the len() function. You can see that how tuples allow duplicate will count event the repeated items.

`Example:`

```python
numbers = ("One", "Two", "Three", "Two", "Three")
print(len(numbers))

# Output:
5
```

## Create Tuple With One Item

To create a tuple with only one item, you have to add a comma after the item, otherwise Python will not recognize it as a tuple.

`Example:`

```python
number = ("One",)
print(type(number))

# Output:
<class 'tuple'>
```

If you forget the comma will be other type:

```python
number = ("One")
print(type(number))

# Output:
<class 'str'>
```

## Tuple Items - Data Types

Tuple items can be of any data type:

```python
set1= (True, True, False)
set2= ("apple", "pineapple", "grapes")
set3 = (5, 10, 15, 20, 25)
print(set1,set2,set3)
```

`Output:`

```python
(True, True, False) ('apple', 'pineapple', 'grapes') (5, 10, 15, 20, 25)
```

## The tuple() Constructor

It is also possible to use the tuple() constructor to make a tuple.

`Example:`

```python
fruits = tuple(("banana", "cherry", "strawberry"))
print(fruits)
```

`Output`:

```txt
('banana', 'cherry', 'strawberry')
```
