# For loop

With this function we can execute a set of statements. It is used when you need to check in a condition each iteration, or to repeat a block of code.

`Example:`

```python
countries = ["Spain", "France", "Italy", "Greece"]
for country in countries:
        print(country)
```

`Output:` As a result are displayed one by one the items.

```python
Spain
France
Italy
Greece
```

## Break statement

With this statement we can stop the loop before finish.

`Example:`

```python
countries = ["Spain", "France", "Italy", "Greece"]
for  x in countries:
        print(x)
        if x == "Italy":
            break
```

`Output:` You can see here that in this time we cannot see "Greece" like in the other example, because the function exit the loop when comply the condition.

```python
Spain
France
Italy
```

## Continue statement

This one is similar to the other, the different is that we can stop the current iteration of the loop and continue with the next.

`Example:`

```python
countries = ["Spain", "France", "Italy", "Greece"]
for  x in countries:
    if x == "France":
        continue
    print(x)
```

`Output:` We can see that "France" is not present.

```python
Spain
Italy
Greece
```

## Looping through a string

With this function we can print each letter of a string in a single line after the loop.

`Example:`

```python
for x in "France":
  print(x)
```

`Output`:

```python
F
r
a
n
c
e
```

There is only 1 letter in every line.

## The range() function

This function returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and ends at a specified number.

### Syntax

 `range(start, stop, step)`

- `start` = Optional.Default is 0.
- `stop` = Required. An integer number specifying at which position to stop (not included).
- `step` = Optional. Default is 1.

`Example:`

```python
for x in range(6):
  print(x)
```

`Output`: We can see here that for default is counting one by one, start in 0 and finished in 5 because was the only value that we define.

```txt
0
1
2
3
4
5
```

This could be a little different if we define every value by adding two additional parameter. I mean, start and step.
In this example i will define ever value so it will star in the number 5, it will sop in the number 30 and will be counting from five to five:

```python
for x in range(5,30,5):
  print(x)
```

`Output`:

```python
5
10
15
20
25
```

## Else in For Loop

The else keyword in a for loop specifies a block of code to be executed when the loop is finished. 

`Example` - Print all numbers from 0 to 4, and print a message when the loop ends:

```python
for x in range(4):
  print(x)
else:
  print("Time to start!")
```

`Output`:

```txt
0
1
2
3
Time to start!
```

`Note: The else block will NOT be executed if the loop is stopped by a break statement.`

`Example` - Break the loop when x is "Three":

```python
numbers =  ["One", "Two", "Three", "Four"]
for x in numbers:
     if x == "Three":
       break
     print(x)
else:
     print("Hello everyone!")
```

`Output`: You can see what happens with the else block, as a result is not executed.

```python
One
Two
```

## The pass statement

- For loops `cannot be empty`, but if you for some reason have a for loop with no content, use the `pass` statement to avoid getting an error.
- The pass statement is a null operation; nothing happens when it is executed.
- The pass is also useful in places where your code will eventually go, but has not been written yet.

`Example:`

```python
numbers =  ["One", "Two", "Three", "Four"]
for x in numbers:
     if x == "Three":
      pass
     print(x)
else:
     print("Hello everyone!")
```

`Output`: But is don't use the pass statement, the code will have an error and don't will be executed.

```python
One
Two
Three
Four
Hello everyone!
```

## Nested Loops 

A nested loop is a loop inside a loop.

`Example:`

```python
color = ["White", "Black", "Brown"]
animal = ["dog", "cat", "mouse"]
for x in color:
  for y in animal:
    print(x, y) 
```

`Output`:

```python
White dog
White cat
White mouse
Black dog
Black cat
Black mouse
Brown dog
Brown cat
Brown mouse
```
