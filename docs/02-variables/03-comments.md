# Comments

Comments do not do anything. Python ignores them. That makes them useful for writing notes in plain English, or whatever language you use, directly in your code.

## Single-line comments

A single `#` makes the rest of the line a comment:

```python
# speed describes how fast the player
# moves in meters per second
speed = 2
```

## Multi-line comments

You can also use triple quotes to write a longer comment, sometimes called a [docstring](https://peps.python.org/pep-0257/):

```python
"""
    the code found below
    will print 'Hello, World!' to the console
"""
print("Hello, World!")
```

This is useful when you want to write a paragraph of comments without putting `#` at the start of every line.
