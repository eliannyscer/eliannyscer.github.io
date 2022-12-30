---
title: "How to install Python on Windows and set path variable?"
tags:
  - Python question
---

* [Install python](https://www.python.org/downloads/)
* After that, install it on your PC. Look for the location where PYTHON has been installed using the following command on your command prompt: `cmd python`.
* Then go to advanced system settings and add a new variable and name it as `Python_name` and paste the copied path.
* Look for the path variable, select its value and select 'edit'.
* Add a semicolon towards the end of the value if it’s not present and then type '%PYTHON_HOME%'

## Additional information

### How to install python on linux?

* To see which version of Python 3 you have installed, open a command prompt and run

```python3
python3 --version
```

* If you are using Ubuntu 16.10 or newer, then you can easily install Python 3.6 with the following commands:

```python
sudo apt-get update
sudo apt-get install python3.6
```
