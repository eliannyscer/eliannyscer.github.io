---
title: "Is python case sensitive?"
tags:
  - Python question
---

Yes. Python is a case sensitive language. Example, if a variable is named ‘HelloWorld‘, then an error will occur if the variable is called ‘helloworld‘. Variables, functions and objects in Python must be called exactly how they are named.

`Example:`

This is the correct way to do it

```python
name = "Ellie."
age = "30"
print("My name is", name + "I am ", age, "years old!")

#Output:
My name is Ellie.I am  30 years old!
```

Now, what happen if you misspell or use capital instead of lower case?

```python
name = "Ellie."
age = "30"
#I am writing "age" with capital letter
print("My name is", name + "I am ", Age, "years old")

#Output:
NameError: name 'Age' is not defined
```

## Reference

[Python case sensitive](https://compscicentral.com/is-python-case-sensitive-answer-example-tips/)