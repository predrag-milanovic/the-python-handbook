# F-Strings in Python

Have you ever played an old-school Pokemon game and given a character a funny name just to make the dialogue more entertaining?

Python has a simple way to build strings that include changing values. It's called an f-string.

```python
num_bananas = 10
bananas = f"You have {num_bananas} bananas"
print(bananas)
# You have 10 bananas
```

To make an [f-string](https://docs.python.org/3/tutorial/inputoutput.html#formatted-string-literals), put an `f` before the opening quote:

```python
f"this is easy!"
```

Use curly brackets `{}` around a variable to [interpolate](https://en.wikipedia.org/wiki/String_interpolation) its value into the string:

```python
name = "Predrag"
print(f"Hello, {name}!")
```

You can also use an f-string directly inside `print()` without assigning it to a variable first. It is still just a string, so there is no need to overthink it.
