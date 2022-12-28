# Strings

Strings can be created by enclosing characters inside a single quote or double-quotes and the output will be the same. They are immutable, you can't modify the content.

`Example:`

```python
'Hello' is the same that "Hello" 
```

`This is not correct:`

```python
"Hello Everyone'
```

You can't mix both quotes as start to write with single quote and close with double.

## To assign string to a variable

Assigning a string to a variable is done with the variable name followed by an equal sign and the string.

`Example:`

```python
name = "Ellie"
print(name)
Ellie
```

## Check string

To check if a  phrase or character is present in a string, we can use `the keyword in`.

`Example:`

```python
phrase= "To have a good life you only need to be happy"
print("good life" in phrase)
True
print("bad life" in phrase)
False
```

## Check if NOT

To check if a  phrase or character is `NOT` present in a string, we can use `the keyword not in`.

`Example:`

```python
a = "Your are learning python"
print("python" not in a)
False
```

The check function it's very useful when you need to check long text:

```python
definition = ("Python is an interpreted, high-level and general-purpose programming language. Python's design philosophy emphasizes code readability with its notable use of significant whitespace. Its language constructs and object-oriented approach aim to help programmers write clear, logical code for small and large-scale projects.")

print("logical code" in definition)
True
print("to help" not in definition)
False
```

## Delete string

To be able to remove the string entirely you new to use the `del` keyword.

`Example:`

```python
name = "Ellie"
del name
print(name)

Traceback (most recent call last):
File "<stdin>", line 1, in <module>
NameError: name 'name' is not defined
```

## Change string

Strings are immutable. This means that elements of a string cannot be changed once they have been assigned. We can simply reassign different strings to the same name.

`Example:`

```python
name = "Louis"
name = "Ellie"
print(name)
Ellie
```

## String Length

To get the length of a string, use the len() function.

`Example:`

```python
names = "Louis and Peter"
print(len(names))
15

b = "You are learning programming"
print(len(b))
28
```

## Multiline Strings

Are delimited by `3 quotes` characters and the new lines are represented by the `\n`. You can use single o double quotes.

`Example:`

```python
"""This is
a multiline
string"""
'This is\na multiline\nstring'
```
