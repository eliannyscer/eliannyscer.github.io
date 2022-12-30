---
title: "What is monkey patching in Python?"
tags:
  - Python questions
---

It is a dynamic (run-time) technique in Python by which you can modify the behavior of an existing class or module.

`In short words refers to dynamic modifications of a class or module at run-time`.

Monkey patching can only be done in dynamic languages.

`Example` - Monkey Patching Python Class:

```python
class monkey:
    def monkeyFunc(self):
        print("my function")
         
def patchFunc():
    print("patching on monkey")
     
 
#normal class method call
objMonkey= monkey()
objMonkey.monkeyFunc()
 
#calling class method after monkey patch
objMonkey.monkeyFunc=patchFunc
objMonkey.monkeyFunc()

# Output:
my function
patching on monkey
```

## Additional information

`Dynamic programming language`

In computer science, a dynamic programming language is a class of high-level programming languages, which at runtime execute many common programming behaviors that static programming languages perform during compilation.

## Reference

[Monkey Patching in Python](https://www.geeksforgeeks.org/monkey-patching-in-python-dynamic-behavior/)

[Dynamic programming language](https://en.wikipedia.org/wiki/Dynamic_programming_language)

[What’s the use of monkey patching?](https://www.csestack.org/monkey-patching-python-coding-example/)
