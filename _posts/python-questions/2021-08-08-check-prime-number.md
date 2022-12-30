---
title: "How to check if a number is prime?"
tags:
  - Python exercise
---

```python
number = int(input("Write a number: ")
  
# If given number is greater than 1
if number > 1:
  
    # Iterate from 2 to n / 2
    for e in range(2, int(number/2)+1):
  
        # If num is divisible by any number between
        # 2 and n / 2, it is not prime
        if (number % e) == 0:
            print(number, "is not a prime number")
            break
    else:
        print(number, "is a prime number!")

# Output:
11 is a prime number!
```

## Additional information

`Prime number` - It is a positive natural number that has only two positive natural number divisors, the number one and the number itself.

* The number `1` is not a prime number by definition, it has only one divisor.

* The number `0` is not a prime number, it is not a positive number and has infinite number of divisors.

`Example:` - The number 13 has only two divisors of 1,13:

```text
13/1 = 13
13/13 = 1
```

`Example:` - The number 15 is not a prime number, thi has more than 2 divisors:

```txt
15/1 = 15
15/3 = 5
15/5 = 3
15/15 = 1
```

`List of prime numbers up to 100:`

```txt
2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97, ...
```

## References

[Prime numbers](https://www.rapidtables.com/math/number/prime_numbers.html)

[Program to check if a number is prime](https://www.geeksforgeeks.org/python-program-to-check-whether-a-number-is-prime-or-not/)

[Program to check if a number is prime using input](https://www.tutorialspoint.com/python-program-to-check-if-a-number-is-prime-or-not)
