---
title: "Dictionary"
tags:
  - Python
---

{% include video id="vIiFpaTpAr0" provider="youtube" %}

It's a fundamental data structure in python, are mutable and we can always add new items after the dictionary has been created.

The `dict()` function creates a dictionary.

Here we will use a dictionary to create a simple phone book.
 You can create,add new names or modify existing ones.

`Example:`

```python
phone_book= {'Mary': '642-534-678','Carlos':'623-678-903', 'Eli': '610-678-234'}
print(phone_book)
```

`output:`

```txt
{'Mary': '642-534-678', 'Carlos': '623-678-903', 'Eli': '610-678-234'}
```

Other way to do it is in different lines, in my opinion this is a more comfortable way because you can see better the details.

`Example:`

```python
phone_book= {
    'Mary': '642-534-678',
    'Carlos':'623-678-903',
    'Eli': '610-678-234'
}
print(phone_directory)
```

## Adding new items in a Dictionary

Adding an item to the dictionary is done by using a new  key and assigning a value to it.

`Example:`

```python
phone_book= {'Mary': '642-534-678','Carlos':'623-678-903', 'Eli': '610-678-234'}
# Add new item
phone_book['Louis'] = '612-987-564'
print(phone_book)
```

`Output:`

You can see as a result how the new item "louis" was added to the phone book:

```txt
{'Mary': '642-534-678', 'Carlos': '623-678-903', 'Eli': '610-678-234', 'Louis': '612-987-564'}
```

## Change Values in a Dictionary

You can change the value of a specific item using the same key name.

`Example:`

```python
phone_book= {'Mary': '642-534-678','Carlos':'623-678-903', 'Eli': '610-678-234'}
#Replace item
phone_book['Mary']= '988-034-567'
print(phone_book)
```

`Output:`

You can se how the item "mary" was replaced for the new number:

```txt
{'Mary': '988-034-567', 'Carlos': '623-678-903', 'Eli': '610-678-234', 'Louis': '612-987-564'}
```

## Duplication Not Allowed

Dictionaries cannot have two items with the same key because the duplicate values will overwrite existing values.

`Example:`

```python
objet= {"Price": "3$", "Name":"pen", "Color":"Black", "Color":"Blue" }
print(objet)
```

Here i'm using a keyword already defined as a result these will be replaced and not added as new:

`Output:`

```txt
{'Price': '3$', 'Name': 'pen', 'Color': 'Blue'}
```

## Dictionary Length

To determine how many items a dictionary has, use the len() function.

`Example:`

```python
objet= {"Price": "3$", "Name":"pen", "Color":"Black" }
print(len(objet))

# Output
3
```

## Update Dictionary

The `update()` function insert items to the dictionary. This items can be a dictionary, or an object. The function it's similar to add new item.

`Example:`

```python
dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
dict.update({"t": "tomato", "b": "banana"})
print(dict)
```

`Output:`

```txt
{'p': 'potato', 's': 'strawberry', 'g': 'grapes', 'a': 'avocado', 't': 'tomato', 'b': 'banana'}
```

## Copy a dictionary

With this function we can copy an existing dictionary. This is the function `copy()`.

`Example:`

```python
dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
food = dict.copy()
print(food)
```

## Check if Key Exists in Dictionary

When you want to determine if a specified key is present in a dictionary you can use the `in` keyword.

`Example:`

```python
dict  =    {
    "Letter p" : "potato",
    "Letter s" : "strawberry",
    "Letter g" : "grapes",
    "Letter a" : "avocado"
}
if "Letter a" in  dict:
    print("Yes, 'Letter a' is in dict! ")
```

`Output:`

```txt
Yes, 'Letter a' is in dict! 
```

## Loop Through a Dictionary

You can loop through a dictionary by using a for loop.

### For loop

Print all key names in the dictionary, one by one with the function `for ... in ..`

`Example:`

```python
dict  =    {
    "Letter p" : "potato",
    "Letter s" : "strawberry",
    "Letter g" : "grapes",
    "Letter a" : "avocado"
}
for dict in dict:
    print(dict)
```

`Output:`

```txt
Letter p
Letter s
Letter g
Letter a
```

### Value function

We can use this function `values()` to return values of a dictionary.

`Example:`

```python
dict  =    {
    "Letter p" : "potato",
    "Letter s" : "strawberry",
    "Letter g" : "grapes",
    "Letter a" : "avocado"
}
for dict in dict.values():
    print(dict)
```

`Output:`

```txt
potato
strawberry
grapes
avocado
```

### Items function

To have both,keys and values, use the `items()` function.

`Example:`

```python
dict  =    {
    "Letter p" : "potato",
    "Letter s" : "strawberry",
    "Letter g" : "grapes",
    "Letter a" : "avocado"
}
for dict in dict.items():
    print(dict)
```

`Output:`

```txt
('Letter p', 'potato')
('Letter s', 'strawberry')
('Letter g', 'grapes')
('Letter a', 'avocado')
```

## Nested Dictionaries

This mean that the dictionary contain many dictionaries. Example, we are going to create a dictionary that contain 3 dictionaries.

`Example:`

```python
my_pets=  {
  "pet1" : {
    "name" : "choky",
    "year" : 2016
  },
  "pet2" : {
    "name" : "cate",
    "year" : 2018
  },
  "pet3" : {
    "name" : "micky",
    "year" : 2019
  }
} 
print(my_pets)
```

`Output:`

```txt
{'pet1': {'name': 'choky', 'year': 2016}, 'pet2': {'name': 'cate', 'year': 2018}, 'pet3': {'name': 'micky', 'year': 2019}}
```

## Remove items from a dictionary

Not only we can modify the items, we can also remove characters from the dictionary that we don't want. There are several methods to do it:

### Pop function

The `pop()` method removes the item with the specified key name.

`Example:`

```python
dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
dict.pop ("g")
print(dict)
```

`Output:`

```txt
{'p': 'potato', 's': 'strawberry', 'a': 'avocado'}
```

### Pop item function

The `popitem()` method removes the last inserted item (in versions before 3.7, a random item is removed instead).

`Example:`

```python
dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
dict.popitem()
print(dict)
```

`Output:`

```txt
{'p': 'potato', 's': 'strawberry', 'g': 'grapes'}
```

### Del function

The `del` keyword removes the item with the specified key name.

`Example:`

```python
dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
del dict["p"]
print(dict)
```

`Output:`

```python
{'s': 'strawberry', 'g': 'grapes', 'a': 'avocado'}
```

`This function can also delete the dictionary completely`. 

This will cause an error because "dict" no longer exists.

`Example:`

```python
dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
del dict
print(dict)
```

### Clear

The `clear()` keyword is used to empty the dictionary.

`Example:`

```python

dict  =    {
    "p" : "potato",
    "s" : "strawberry",
    "g" : "grapes",
    "a" : "avocado"
}
dict.clear()
print(dict)

#Output
{}
```
