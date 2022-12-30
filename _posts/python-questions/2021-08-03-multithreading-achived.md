---
title: "How is Multithreading achieved in Python?"
tags:
  - Python FAQ
---

* Python has a construct called the `Global Interpreter Lock` (GIL). The GIL makes sure that only one of your `threads` can execute at any one time. A thread acquires the GIL, does a little work, then passes the GIL onto the next thread.

* This happens `very quickly` so to the human eye it may seem like your threads are executing in parallel, but they are really just taking turns using the same CPU core.

* All this GIL passing adds overhead to execution. This means that if you want to make your code run faster then using the threading package often isn’t a good idea.

## Additional information

`Multithreading` - It is defined as the ability of a processor to execute multiple threads concurrently.
Python has a multi-threading package but if you want to multi-thread to speed your code up then it’s usually not a good idea to use it.

`What is Thread?` - It is a sequence of instructions that operating system executes independently. Using several threads in parallel we can improves execution time and can be very useful when we need to perform multiple tasks at the same time.

## References

[Multithreading](https://www.quora.com/How-is-multithreading-achieved-in-Python-Whenever-Python-exits-why-isn-t-all-the-memory-deallocated?share=1)

[What is Thread?](https://www.simplifiedpython.net/python-threading-example/)
