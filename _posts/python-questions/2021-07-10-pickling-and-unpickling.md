---
title: "What is pickling and unpickling?"
tags:
  - Python question
---

## Pickling

It is a process of converting a `object` into a `bytes stream` and  it is bstored into a file.

## Unpickling

It is inverse operation of pickling. Unpickling is a process where a `byte stream` is converted back into a `object`.  

## Additional information

It is primarily used in serializing and deserializing a Python object structure. In other words, it's the process of converting a `Python object` into a `byte stream` to store it in a file/database, maintain program state across sessions, or transport data over the network.

## Pickling - Explanation

* It is a process of converting a `object` into a `bytes stream` and  it can be stored into a file,this process also called as object serialization.

* It a module (you need to import before use).
  
* You need to use `dump function` from pickle module.

`Example:`

```python
import pickle

# Python object
my_list = [30, "Python", b"I love Python"]

# Pickling
with open("data.pickle","wb") as file_handle:
    pickle.dump(my_list, file_handle, pickle.HIGHEST_PROTOCOL)

print("Pickling completed!")

# Output:
Pickling completed!
```

## Unpickling - explanation

* It is inverse operation of pickling. Unpickling is a process where a `byte stream` is converted back into a `object`.  

* This process is also called as de-serialization.

* You need to use `load()` function from pickle module, which is used to read an pickled object from a binary file and returns it into an object.

`Example:`

```python
import pickle

# Pickling
with open("data.pickle","rb") as file_handle:
    retrieved_data = pickle.load(file_handle)
    print(retrieved_data)

# Output:

[30,"Python", b"I love Python"]
```

## References

[Pickling and unpickling](https://askinglot.com/what-is-pickling-and-unpickling-in-python)

[Definitions](https://codingisfuture.com/python/pickling-and-unpickling/)

[Examples](https://www.codesansar.com/python-programming/what-is-pickling-and-unpickling.htm)
