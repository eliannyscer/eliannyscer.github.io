---
title: "
Whenever Python exits, why isn’t all the memory de-allocated?"
tags:
  - Python FAQ
---

Python modules are not always de-allocated when Python exits.

`Explanation:`

* The modules with circular references to other objects, or to objects referenced from global namespaces, aren’t always freed on exiting Python.

* Plus, it is impossible to de-allocate portions of memory reserved by the C library.

* On exit, because of having its own efficient cleanup mechanism, Python would try to de-allocate/destroy every other object.

## References

[Memory de-allocated](https://www.edureka.co/community/10857/whenever-you-exit-python-is-all-memory-de-allocated)

[Releasing Memory](http://net-informations.com/python/iq/memory.htm)