---
title: "How to check if a sequence is a Palindrome?"
tags:
  - Python exercise
---

A string is said to be palindrome if the reverse of the string is the same string.

`Example:`

```text
Input: level
Output: Yes

Input: civic
Output: Yes

Input: Ellie
Output: No
```

## Program

`Example:` - Using one extra variable:

```python
word = "Ellie"
 
result = ""
for w in word:
    result = w + result
 
if (word == result):
    print(f 'The word "{word}" is palindrome')
else:
    print(f 'The word "{word}" is not palindrome')

# Output:
The word "Ellie" is not palindrome
```

In this method user take a character of string one by one and store in an empty variable. After storing all the character user will compare both, the string and check it is palindrome or not.

`Example` - This method is case sensitive:

```python
word = "Level"
 
result = ""
for w in word:
    result = w + result
 
if (word == result):
    print(f'The word "{word}" is palindrome')
else:
    print(f'The word "{word}" is not palindrome')

# Output:
The word "Level" is not palindrome
```

Even when the word is palindrome the output is opposite, this because the first letter of the word is capital an this method is case sensitive.

## Reference

[Examples](https://www.geeksforgeeks.org/python-program-check-string-palindrome-not/)

[Palindrome words](https://www.rd.com/list/palindromes-list/)
