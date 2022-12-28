# Mad libs

According to Wikipedia, "Mad Libs is a phrasal template word game where one player prompts others for a list of words to substitute for blanks in a story before reading aloud."

It's a game where you can answer about random words (verbs, nouns, names) and you take this words and put in a story, randomly.

## How word the game?

1.There is a story that has many key words replaced with blanks.

2.Each blank is specified a category, such as exclamation, noun, a verb like that.

3.You ask another player to contribute a word of the specified type for each blank, but without revealing the context for that word.

4.Finally, after filling all the blanks with the parts of speech given by that another player, the completed story is read aloud.
  
`The result is usually comic, surreal, and somewhat nonsensical 😆.`

## What you will learn?

By doing this simple project, you will learn the following:

1.How to `run` a python file in the Terminal

2.How to work with `string` data type in python

3.The concepts of `variables`

4.How to take `input` from the user

5.And how to `output` something to the screen

## Getting Started

The first thing we need to do is to prompt the user to type something and take the input from the user, right? We can do that using input() function like this.

```python
input("What is your name?")
```

This function will throw whatever message you put inside those () brackets onto the screen and takes whatever the user types as input until they hit the Enter key.

So let's store the value the user had entered in a variable called "name" and try to print() it back to the screen.

`To output something to the screen, we use the print() function.`

```python
name = input("What is your name? ")
print(name)
```

## The Actual Game

Now let's create the Madlibs game.

In our story, we need 3 parts of speech / in our case 4 variables namely:

Felling
Place
Food

So we are going to prompt the user to input them and store them in the corresponding variables. Type the following code into the mad libs.py file:

We need to create 3 variables, called (Felling, place and food ) in this form the user can write inside this variable.

```python
felling = input ("Enter a felling: ")
place = input ("Enter a place: ")
food = input ("Enter a food: ")

print("Today i fell " + felling )
print("because yesterday i was in the " + place)
print("eating " + food)
```

## F-string

We can do it in form too, just put an f before the string and use {} to reserve spaces. Then inside the {}, we can put whatever variable we need and its value will get replaced. And it's more readable too.

```python
print(f"Today i fell {felling} because yesterday i was in the {place} eating {food}")

or

felling = input ("Enter a felling: ")
place = input ("Enter a place: ")
food = input ("Enter a food: ")

print(f"Today i fell {felling}")
print(f"because yesterday i was in the {place}")
print(f"eating {food}")
```

`After read this information your homework is create your onw mad lip`. 

Hopefully will be more funny than mine!