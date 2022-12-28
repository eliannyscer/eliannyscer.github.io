---
title: "While Loops"
categories:
- Programming
tags:
- Python
---
{% include video id="RT8YgqoY234" provider="youtube" %}

With the while loop we can execute a set of statements as long as a condition is true.

## Syntax

```python
while expression:
    statement(s) / Body of the while loop
```

`Example:`

```python
num = 0
while num <= 7:
    print(num)
    num = num + 1 (This is same: num += 1)
```

To increment the value of the “num” variable is very important because, without incrementing the value of num, our Loop will never end and will go to the infinity

## One-Line while loop

`Example:`

```python
num = 0
while num < 7: print(num); num += 1 
# Or 
while num < 7: print(num); num = num + 1
```

`In both cases (While loop and one-line while loop) the output will be the same`

Output:

```txt
0
1
2
3
4
5
6
7
```

## The Infinite Loop

A loop becomes infinite loop if a condition never becomes `FALSE`.
So there is no guarantee that the loop will stop unless we write the necessary code to make the condition False at some point during the execution of the loop. This results in a loop that never ends.

`Example:`

```python
num = 2
while num == 2:
    print("This is Infinite Loop")

Output:

This is Infinite Loop
This is Infinite Loop
This is Infinite Loop
This is Infinite Loop
This is Infinite Loop
This is Infinite Loop

```

`You need to use CTRL+C to exit the program`.

The condition num = 2 is always True so the loop never stops.If you want different result, you need to write a condition.

`Example:`

```python
num = 2
while num == 2:
    print("Infinite")
    num += 1

# Output:
Infinite
```

## Using else Statement with While Loop

If the else statement is used with a while loop, the else statement is executed when the condition becomes false.

The following example illustrates the combination of an else statement with a while statement that prints a number as long as it is less than 5, otherwise else statement gets executed.

`Example:`

```python
i = 1
while i < 6:
    print(i)
    i += 1
else:
    print("i is no longer less than 6")

# output:
1
2
3
4
5
i is no longer less than 6
```

## Loop control statements - While loop

## Statements break and continue

`BREAK` is used to stop the loop even if the while condition is true while with  `CONTINUE` we can stop the current iteration, and continue with the next. Here are some examples:

## Continue

It is used to exit the Loop.

`Example:`

```python
num = 0
while num <7:
    num += 1
    if num == 5:
        continue
    print(num)
```

`output` - The `continue` statement is executed and as a result the number 5 is skipped from the count.

```python 
1
2
3
4
6
7
```

## Break

```python
num = 0
while num < 5:
    num += 1
    if num == 4:
        break
    print(num)
```

`Output` - The `break` instruction is executed and as a result the program stops executing with the number four.

```python
1
2
3
```

## Pass

It is not considered as a declaration of operation. It is more like a comment but it is executed as a valid statement although it is completely ignored. It is generally used to indicate nullity.

`Example:`

```python
num = 0
while num < 7:
    num += 1
    if num == 5:
        pass
    print(num)
```
