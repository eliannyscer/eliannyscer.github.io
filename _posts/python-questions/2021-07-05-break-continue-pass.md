---
title: "How does break, continue and pass work?"
tags:
  - Python questions
---

* `Break` - It finish the current loop. Use the break statement to come out of the loop instantly.

* `Continue` - Skip the current iteration of a loop and move to the next iteration.

* `Pass` - The pass statement is a null operation; nothing happens when it executes.

## More information

Everyone can be used with `for` an `while` loop.

## Breaks

`Example-` Break statement in a `for loop`:

* If we found a number greater than 100, we will `break` the loop.

* Use the `if` condition `to terminate` the loop. If the condition evaluates to `true`, then the loop will terminate. The loop will continue  until the main loop condition is true.

```python
numbers = [30, 60, 90, 120]
for n in numbers:
    if n > 100:
        break
    print("Current number:", n)

#Output:
Current number: 30
Current number: 60
Current number: 90
```

`Note:` As you can see in the output, we got numbers less than 100 because we used the break statement inside the if condition (the number is greater than 100) to terminate the loop.

## Continue

Use the if condition with the continue statement. If the condition evaluates to true, then the loop will move to the next iteration.

`Example-` Continue statement in a `for loop`:

```python3
for e in "Ellie":
    if e == "i" :
        continue
    print("Letter:", e)

#Output:
Letter: E
Letter: l
Letter: l
Letter: e
```

As you can see in the output, the condition become `true` then the loop skipped the letter `"i" and continue printing the last one.

## Pass

This is null, ignore the condition and proceed to run the program as usual. The pass is also useful in places where your code will eventually go, but has not been written yet.
It is used when a statement is required syntactically but you do not want any command or code to execute.

`Example-` Pass statement in a `for loop`:

```python
week_days = ["Monday", "Tuesday", "Wednesday"]
for wd in week_days:
    pass
print(week_days)

#Output:
['Monday', 'Tuesday', 'Wednesday']
```

## References

[Pass statement](https://www.tutorialspoint.com/python/python_loop_control.htm)

[Break-Continue-Pass](https://pynative.com/python-break-continue-pass/)

[Examples](https://pynative.com/python-break-continue-pass/#h-how-break-statement-works)
