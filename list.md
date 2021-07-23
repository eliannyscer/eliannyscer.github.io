# List

List in python are containers that can store any type of data that you want

An empty list
We can add the item later

```python
empty = []
```

List of numbers

```python
numbers = [10, 20, 30, 40.5]
```

List of strings

```python
words =["Hello", "Hallo", "Hola", "Labas"]
```

List of mixed items

```python
anything = [10, "Hello", 40.5, "Labas"]
```

Note: A python list is called `Array` in other languages, like JavaScript.

## Index

List item are ordered starting with index (or position) 0:

```python
greetings = ["Hello", "Hola", "Labas", "Hallo"]
              [0]      [1]     [2]      [3]
```

You can also slice a list to get a sub-section of the list:

`For example:` greetings [1:3]

## Creating a List and adding Items

With the function `append()` we can add new items to the end of our list:
list_name.append(item). Let's try:

```python
greetings = ["Hola", "Hello"]
print(greeting)

#output:
['Hola', 'Hello']

greetings = ["Hola", "Hello"]
greetings.append("Labas")
greetings.append("Hallo")
print(greetings)

#Output:
['Hola', 'Hello', 'Labas', 'Hallo']
```

## Removing elements

We can remove items form our list in two ways:

* Using `remove()`

we use this function in the say way that `append()`

```python
greetings = ["Hola", "Hello"]
greetings.remove("Hola")

#Output:
['Hello']
```

* Using `del`

```python
greetings = ["Hola", "Hello"]
del[1]

#Output:
['Hello']
```

We can remove a slice of the list to by using the `del` function:

```python
greetings = ["Hello", "Hola", "Labas", "Hallo"]
del greetings[:2]
print(greetings)

#Output:
['Hallo']
```
