# Dynamic Typing

Python is dynamically typed, which means a variable can store any type, and that type can change.

For example, a variable that starts as a number can later hold a string:

```python
speed = 5
speed = "five"
```

## But Like, Maybe Don't

In almost all circumstances, it is a bad idea to change the type of a variable. The better approach is to create a new variable with a name that matches the new value:

```python
speed = 5
speed_description = "five"
```

This keeps your code easier to read and avoids confusion later.

## What Is Non-Dynamic Typing?

Languages that are not dynamically typed are called [statically typed](https://en.wikipedia.org/wiki/Type_system#Static_typing), such as Go and TypeScript.

In a statically typed language, if you try to assign a value of the wrong type to a variable, you get a compile-time error and the program will not run.

If Python were statically typed, the earlier example would fail on the second line, `speed = "five"`, because a string could not be assigned to a number variable.

Dynamic typing gives Python flexibility, but good variable naming still matters. Usually, the cleanest code is the code that keeps each variable focused on one kind of value.
