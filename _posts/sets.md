# Sets

the collection is mutable and the elements can be added and removed to the set. The set are very similar to the dictionaries, limited by curly brackets but every item is a single objet separated by a colon

Sets are iterable although the order is arbitrary. You can mis letter and numbers.

`Example:`

```python
set = {"apple", "pineapple", "grapes"}
print(set) 
```

`Output:`

```txt
{'pineapple', 'apple', 'grapes'}
```

`Note: Sets are unordered, so you cannot be sure in which order the items will appear.`

## Set Items

- Set items are unordered, unchangeable, and do not allow duplicate values.

- Unordered: Means that the items in a set do not have a defined order. Set items can appear in a different order every time you use them, and cannot be referred to by index or key.

- Unchangeable: Means that we cannot change the items after the set has been created.

## In and not in operator

with this function you can check if a item is present or not in the code using `in` or in `not`.

`Example:`

```python
#in
letters = {"s", "m", 2, "h"}
print(2 in letters)

#in not
letters = {"s", "m", 2, "h"}
print(2 not in letters)
```

`Output` - As a result will be executed answering `True` or `False`:

```python
True
False
```

## Duplicates no allowed

Sets cannot have two items with the same value.

`Example:`

```python
letters = {"s", "m", "s", "h"}
print(letters)
```

`Output` - As a result you will see that the item that al ready exists is not present.

```text
{'m', 's', 'h'}
```

## Add item

Once a set is created, you cannot change its items, but you can add new items.

`Example:`

```python
letters = {"s", "m", 2, "h"}
letters.add("y")
print(letters)
```

`Output` - We have this result because the order is arbitrary in the sets:

```txt
{'h', 2, 'm', 's', 'y'}
```

`Remember, if you add a element that already exist this don't have any effect`

## Update

The update() method updates the current set, by adding items from another set.

If an item is present in both sets, only one appearance of this item will be present in the updated set.

`Example:`

```python
letters = {"s", "m", "a", "h"}
letters.update(["r","w", "u"])
print(letters)
```

`Output:`

```txt
{"a", 's', 'r', 'w', 'u', 'm', 'h'}
```

## Copy

```python
letters = {"s", "m", 2, "h"}
x = letters.copy()
print(x)
```

`Output`:

```txt
{'m', 2, 's', 'h'}
```

## Length

To determine how many items a set has, use the len() method.

`Example:`

```python
letters = {"s", "m, "h"}
print(len(letters))

# Output:
3
```

`if you repeat the same item two times the function will count it only one time`

```python
letters = {"s", "m, "s", "h"}
print(len(letters))

# Output:
3
```

## Remove

With this function y you can delete specific item but delete a items that is not present in the set produce error.

`Example:`

```python
letters = {"s", "m", 2, "h"}
letters.remove("s")
print(letters)
```

`Output:`

```txt
{2, 'h', 'm'}
```

### Error

```python
letters = {"s", "m", 2, "h"}
letters.remove("x")
print(letters)
```

## Discard

The discard() method removes the specified item from the set.

This method is different from the remove() method, because the remove() method will raise an error if the specified item does not exist, and the discard() method will not.

`Example` - Removing existing item:
  
```python

letters = set(("e", "f", "t"))
letters.discard("e")
print(letters)
```

`Example` - Removing an item that doesn't exist:

```python
letters = set(("e", "f", "t"))
letters.discard("h")
print(letters)
```

`Output`- In the first output you can see that the item was removed and in the second one you can see that nothing happened.

```python
{'f', 't'}
{'t', 'e', 'f'}
```

`Output` How the letter "x" don't was present in the set produce a error

```python
KeyError: 'x'
```

## Clear

method doesn't return any value, the result is to have a empty set.

`Example:`

```python
letters = set(("e", "f", "t"))
letters.clear()
print(letters)
```

`Output:`

```txt
set()
```

## Set Items - Data Types

You can mix numbers, letter, word or even you can use true or false.

`Example:`

```python
set1= {True, True, False} 
set2= {"apple", "pineapple", "grapes"}
set3 = {5, 10, 15, 20, 25}
print(set1,set2,set3)
```

`Output:`

```txt
{False, True} {'pineapple', 'grapes', 'apple'} {5, 10, 15, 20, 25}
```

## The set() Constructor

It is also possible to use the set() constructor to make a set. 

`Example:`

```python
letters = set(("e", "f", "t"))
print(letters)
```

`Output`- You can see that i don't was using curly brackets.

```txt
{'f', 'e', 't'}
```
