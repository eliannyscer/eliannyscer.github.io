---
title: "How will you capitalize the first letter of string?"
tags:
  - Python question
---

## Capitalize()

* Convert the first letter in the string in a capital letter.

* Syntax -  `string.capitalize()`.

`Example:`

```python
txt = "hello!"
x = txt.capitalize()
print (x)

# Output:
Hello!
```

`Other Example:`

If there is some capital letter already in your string this function it will make them lowercase.

```python
txt = "heLLO!"
x = txt.capitalize()
print (x)

# Output:
Hello!
```

## Additional information

There is other function similar to `capitalize()` but with a different effect over the string. You should know it.

## Upper

* This method returns a string where all characters are in upper case.

* Syntax - `string.upper()`

`Example:`

```python
txt = "hello, I am ellie!"
x = txt.upper()
print(x) 

# Output:
HELLO, I AM ELLIE!
```

## References

[Capitalize](https://www.w3schools.com/python/ref_string_capitalize.asp)

[Upper](https://www.w3schools.com/python/ref_string_upper.asp)