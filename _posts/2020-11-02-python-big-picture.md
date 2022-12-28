---
title: "Vocabulary"
categories:

  - Blog
tags:
  - Python
---

## Reserved Words

Are special words with special meaning, for example, if you use "Else" there ir not other word that python implement in that way.
 When you use this words python don't allow you to use for other purpose, only the purpose that python want or understand and you can not use this name as a variable.

 `Example:` You are in other country like France with a language different to yours and you try to communicate in your language, probably anybody will understand you, but if you some words in french the people will know what you want or try to said, is the same with this words, if you use in a different way python will not execute your command because don't understand what you want to use if you want use for a different propose.

 For python is like:
 You: Class
 python: I know what that mean.. Execute!

- false and true
- none
- and, as
- assert
- break, continue, pass
- Class
- if, else,elif
- def
- del
- except
- return
- for
- is
- lambda
- while
- not
- or
- raise
- finally
- nonlocal
- with
- yield
- Print

`ǸOTE: If you want to use one of this words like a variable you need to add a number, letter o phrase.`

## Sentence or lines

- Assignment statement
- Assignment with expression
- print statement

```python
e = 25
e = e + 1
print(e)

#Output
26
```

- e = Variable

- 25 y 1 = Constant

- print = Reserved word

- = and + = Operators

Accept the fact that not necessary make sense in the big picture

Variables, Expression and statements

## Constants

- The constants values such a number, letters and strings, are called in this way because their value does not change.
- Numeric `constants` are as you expect
- String `constants` use single or double quotes ('' or "")

Example:

```python
print(195)
195
print(25.1)
25.1
print("Hello everyone")
Hello everyone
```

## Variables

- Is a named place in the memory where a programmer can store data and later retrieve the data using the variables "name"
- The programmer choose the name of the variable
- You can change the content of a variable in other statement
- You can control de variables using the equal sing (`=`)

```python
e = 15
l = "Hello"
i = 26

#OutPut
15
Hello
26
```

`The variable hold only one statements`. You will se in this example that is there is two equal item is execute the new one:


```python
e = 15
l = "Hello"
l = "Hello everyone"
i = 26

#OutPut
15
Hello Everyone
26
```

## Python Variables Names Rules

- Must start with a letter or underscore
- Must consist of letter, numbers, and underscore
- Case sensitive

```python
#Example 
Spain = 
Spain95 = 
```

### choose good variables names will help you to understand whats going on. Example:

`Complicate`

```python
asdfghj1klñ= 40
asdfghj2klñ = 8
asdfghj3klñ = asdfghj1klñ * asdfghj2klñ
print(asdfghj3klñ)

#Output
320
```

`Easy`

```python
e = 40
l = 8
i = e * l
print(i)

#Output
320
```

`Simple` In my opinion the best way to do it is this because is easier to understand what you are doing. So if is possible to do it in this way. Why not? so do it.

```python
hours= 40
earn = 8
salary = 40 * 8
print(salary)

#Output3
320
```

`Every code was doing exactly the same, the different was how we use the variables.`
when you are writhing numbers you need to pay attention to the details because other way python will be `Unhappy` and will not execute your code

## Expresiion

Are a little big more complex calculations 

## Type Matters

- Python know what `type` everything is
- Some operations are prohibited
- You cannot `add 1` to a string
- we can ask Python what type something is by using the `type()` function

In this example you can see that you can not mix a string with a number, as a result you will have an error:

```python
word = "Hello"
word = word + 1 
print(word)

#Output
word = word + 1 
TypeError: can only concatenate str (not "int") to str
```

`If you print the type of everyone you will see that are different or incompatible and for that reason don't was executed:`

```python
word = "Hello"
number = 1
print(type ("Hello"))
print(type(word))
print(type(1))

#Output
<class 'str'>
<class 'str'>
<class 'int'>
```

## User input

- With this function we are able to ask the user for input.
- This function return a string
- We can instruct python to pause and read data from the user using the `input()` function

`Note:` If you want to have a space between the question and the answer you need to leave a space after the question when you are writing the code, other way the question and the answer will be togethers.


```python
country = input ("Where are you from? ")
print("Welcome!")
```

`Output` Python stops executing when it comes to the input() function, and continues when the user has given some input.

```python
##You need to write a answer to continue
Where are you from? Spain
Welcome!
```

## Comments in Python

- Anything after a `#` is ignored by python

### Why use comments?

- Describe what is going to happen in a sequence of code
- Document who wrote the code or other ancillary information
- Turn of a line of code - Perhaps temporarily

```python
country = input ("Where are you from? ")
print("Welcome!")
```

`Output`

```python
##You need to write a answer to continue
Where are you from? Spain
Welcome!
```