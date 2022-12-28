---
title: "Statements"
categories:
- Programming
tags:
- Python
---

Conditional statements allow you to control the flow of your program more effectively.
The statements "In, if and else" evaluate when an expression is true or false. If a condition its true the "if" statements execute.

## If

 The statement will execute a block of code if a specified condition is equal to true. Otherwise, the block of code within the if statement is not executed.
 Let’s write a program that prints the price of shoes in an online store. This command only will work if the customer has ordered a black shoes.

Here is the code for our program:

```python
shoes_order = "black shoes"
if shoes_order == "black shoes":
    print("price: $13.99")
```

Output: `price: $13.99`

Our code returns: $13.99
We use the variable "shoes_order" for the the value "black shoes".

We use an if statement to check that "shoes_order" is equal to "black shoes" .

 If our condition is true, our print() statement is be executed. If our condition is false, nothing will happen.

Now, let’s see what happens when we change our shoes order to white shoes:

```python
shoes_order = "white shoes"
if shoes_order == "black shoes":
    print("price: 13.99")
```

Our code it's not executed, this is because our shoes order is not equal to black shoes.

## If Else

If a condition is true, the if statement executes. Otherwise, the else statement executes.

Suppose we create an application that verifies the use of gift cards, the maximum limit will be $ 40.

If the user exceeds $ 40, he will not be able to continue buying.
If the user has not exceeded that amount, he can continue buying.

`Example:`

```python
card = "15.98$"
if card > "40$":
    print("You have exceeded the limit of your card!")
else:
    print("You can buy more in our store, you still have money in your card!")
```

You can buy more in our store, you still have money in your card!

### `How our code works?`

- First, we declare a Python variable called card. This variable tracks a user card.
- We use an if statement to check when the card is greater than 40.
-If the user card if more than $40, the statement after our "if" clause is executed. Otherwise, the statement after our "else"clause is executed.

## Elif

In some cases, we may want to evaluate multiple conditions and create outcomes for each of those conditions. That’s where the `elif` condition comes in.

They appear after a Python if statement and before an else statement. You can use as many `elif` statements as you want.

`Example` - Suppose that you want to have different prices together. You could use a similar code:

`Orange cake:` $3.99

`Chocolate cookie:` $1.00

`Cheese cake:` There is not available today

`Others cakes:` $2.80

```python
cake_order = "Orange cake"
if cake_order == "Orange cake":
    print("Price: $3.99")
elif cake_order == "Lemon cake":
    print("Price: $1.00")
elif cake_order == "cheese cake":
    print("There is not available today")
else: 
    print("price:$2.80")
```

Output: `price: $3.99`. In general we had 4 possible answers.

If we introduced a new cake to our menu, we can add more elif statements.This new statement could print the price of the new menu item to the console.
