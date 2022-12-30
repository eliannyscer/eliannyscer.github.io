---
title: "What is namespace in Python?"
tags:
  - Python questions
---

Namespaces make our programs immune from name conflicts

* A namespace is basically a system to make sure that all the names in a program are unique and can be used without any problem.
* The name means the name of the variable, space is about the location from where you can access to the variable.
* You can think of a namespace as a dictionary where the names are keys and the objects are values.

`Example`

The role of a namespace is like a surname. Maybe we would not find a single “Ellie” in a class because there is  multiple “Ellie” but when you particularly ask for “Ellie Collins” or “Ellie Clark” (with a surname), there will be only one (Probably).
But what happen if the name and surname are same for multiple students?. The Python interpreter understands what exact method or variable we are trying to find  in the code. `So, the division of the word itself gives a little more information`. Name (means a unique identifier) + Space(the path to the file,the location from where is trying to access a variable or a method).

## Additional information

### Python Variable Scope

Although there are various unique namespaces defined, we may not be able to access all of them from every part of the program. The concept of scope comes into play.

`A scope is the portion of a program from where a namespace can be accessed directly without any prefix.`

At any given moment, there are at least three nested scopes.

*`Scope of the current function ,it has local names`. In this example, I have defined a function vehicle, and the car is the local namespace that is inside the function vehicle.

```python
def vehicle():
    car = "Volkswagen"
    print(car)
vehicle()

Output:
Volkswagen
```

*`Scope of the module which has global names`. In this example, I have defined function vehicle namespace, Bicycle namespace is defined outside the `function()` vehicle, so the `Bicycle = “Himo”` is a global namespace.
It can also be printed inside the function.

```python
Bicycle = "Himo"
def vehicle():
    car = "Volkswagen"
    print("car:",car)
    print("Bicycle:",Bicycle)
    print("Inside the function", Bicycle)
vehicle()

Output:
car: Volkswagen
Bicycle: Himo
Inside the function Himo
```

*`Outermost scope which has built-in names`. A built-in namespace contains the built-in functions like print(), open(), close(). In this example, I am not defining any function print is a built-in namespace in python.

```Python
print("Ellie")

Output:
Ellie
```

## Summary

* When a reference is made inside a function, the name is searched in the local namespace, then in the global namespace and finally in the built-in namespace.

* If there is a function inside another function, a new scope is nested inside the local scope.
Some functions like print(), id() are always present, these are built-in namespaces.

* When a user creates a module, a global namespace is created, later the creation of local functions creates the local namespace.
