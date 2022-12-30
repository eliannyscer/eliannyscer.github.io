---
title: "What is the difference between list and tuples in Python?"
tags:
  - Python question
---

## LIST

`Type` - Are mutable (can be edited), it is possible update or delete an item from the list.

`Iteration` - It is slower than tuples.

`Syntax` - You use square bracket.

`Example:`

```python3
supermarket_list = ["Cereal", "bread", "avocado", "beef"]
print(supermarket_list)

# Output:
# ['Cereal', 'bread', 'avocado', 'beef']
```

## TUPLES

`Type` - Are immutable, if you try to modify as a result you will have an error. For example if you try to delete some item you will get an error instead yu have to assign it to a new Tuple. 

`Iteration` - It is faster than list.

`Syntax` - You use round brackets.

`Example:`
  
```python3
supermarket_list = ("Cereal", "bread", "avocado", "beef")
print(tuple)

# Output:
# ('Cereal', 'bread', 'avocado', 'beef')
```

## References

[Differences](https://www.tutorialspoint.com/difference-between-list-and-tuples-in-python)

[Similarities](https://www.tutorialspoint.com/What-are-the-differences-and-similarities-between-tuples-and-lists-in-Python)

[How to add Elements to a List in Python](https://www.journaldev.com/33182/python-add-to-list)

[How to add new items to tuple in Python](https://www.codespeedy.com/add-new-items-to-tuple-in-python/)

[Remove item from a tuple](https://www.tutorialgateway.org/python-program-to-remove-an-item-from-tuple/)