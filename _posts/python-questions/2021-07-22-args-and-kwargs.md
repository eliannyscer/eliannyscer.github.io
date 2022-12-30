---
title: "What does this mean: *args, **kwargs? And why would we use it?"
tags:
  - Python FAQ
---

Putting `*args` and/or `**kwargs` as the last items in your function definition’s argument list `allows` that function to accept an `arbitrary` number of arguments and/or keyword arguments.

You don’t actually have to call them `args` and `kwargs`, that’s just a convention. It’s the `*` and `**` that do the magic.

In other words we can pass a variable number of `arguments` to a `function` using special symbols (there are two special symbols).

## *args - (Non-Keyword Arguments)

* Allows you to take  more arguments than the number of formal arguments that you previously defined.

* Using the `*`, the variable that we associate with the `*` becomes an iterable.

`Example:`

```python
def myFun(*argv):
    for arg in argv:
        print (arg)
   
myFun("You", "are", "learning", "something", "new", "today!")

# Output:
You
are
learning
something
new
today!
```

## **kwargs - (Keyword Arguments)

We use with double star. The reason is because the double star allows us to pass through keyword arguments (and any number of them).

A keyword argument is where you provide a name to the variable.

`Example:`

```python
def myFun(**kwargs):
    for key, value in kwargs.items():
        print ("%s == %s" %(key, value))
 
myFun(First = "Hello!", Second = "I am", Third= "Ellie")  

# Output:
First == Hello!
Second == I am
Third == Ellie
```

## References

[*args and **kwargs](https://www.geeksforgeeks.org/args-kwargs-python/)

[Official python documentation](https://docs.python.org/2/tutorial/controlflow.html#more-on-defining-functions)

[What do *args and **kwargs mean?](https://stackoverflow.com/questions/287085/what-do-args-and-kwargs-mean)
