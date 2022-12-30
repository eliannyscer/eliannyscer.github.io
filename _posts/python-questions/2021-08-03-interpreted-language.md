---
title: "Python is interpreted language. what does it mean?"
tags:
  - Python question
---

## Interpreted vs compiled language

An interpreter executes the statements of code “one-by-one” while the compiler executes the code entirely and lists all possible errors at the same time time.

### Interpreted (Python, ruby, JavaScript)

*Interpreted language run through a program line by line and execute each command

*In interpreted language, every single line is converted to machine code directly. That's why Python is very slow, because it interpret one line at a time

* Display error when each instruction is run. Python shows only one error message even though your code has multiple errors. This will help you to clear errors easily and it definitely will increase the execution speed

### Compiled( C, C**, Pascal)

*In compilation, source code is first converted to object code and then to the machine code

* Compilation is the process of translating code from language A to language B (Language -> Machine code)

* Display errors once the entire program is checked

`Example:`

Imagine you have a hummus recipe that you want to make, but it's written in ancient Greek. There are two ways you, a non-ancient-Greek speaker, could follow its directions

The first is if someone had already translated it into English for you. You (and anyone else who can speak English) could read the English version of the recipe and make hummus. Think of this translated recipe as the compiled version

The second way is if you have a friend who knows ancient Greek. When you're ready to make hummus, your friend sits next to you and translates the recipe into English as you go, line by line. In this case, your friend is the interpreter for the interpreted version of the recipe