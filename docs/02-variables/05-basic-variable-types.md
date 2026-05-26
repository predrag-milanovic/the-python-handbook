# Basic Variable Types

Python has a few basic [data types](https://en.wikipedia.org/wiki/Data_type) you'll use all the time.

## Strings

Strings are snippets of text. They are made up of characters joined together.

When you create a [string](https://docs.python.org/3/library/stdtypes.html#textseq), wrap the text in single quotes or double quotes. In Python style, double quotes are usually preferred:

```python
name_with_single_quotes = 'boot.dev'  # not as common
name_with_double_quotes = "boot.dev"  # preferred
```

## Numbers

Numbers are not surrounded by quotes.

An [integer](https://docs.python.org/3/c-api/long.html), or `int`, is a whole number with no decimal part:

```python
x = 5   # positive integer
y = -5  # negative integer
```

A [float](https://docs.python.org/3/library/functions.html#float) is a number with a decimal part:

```python
x = 5.2
y = -5.2
```

## Booleans

A [Boolean](https://docs.python.org/3/c-api/bool.html#boolean-objects), or `bool`, can only have one of two values: `True` or `False`.

These values are useful any time your code needs to answer a yes-or-no question:

```python
is_tall = True
is_short = False
```

Booleans are a core part of how computers represent logic. At a low level, they map cleanly to the idea of 1s and 0s, which makes them perfect for decisions in code.
