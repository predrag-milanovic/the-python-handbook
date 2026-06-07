# Exponents

Python has built-in support for exponents, which is something many other languages require a `math` library for.

Use the `**` operator to raise a number to a power:

```python
# Reads as "three squared" or
# "three raised to the second power"
3 ** 2
# 9
```

Sometimes exponents are written in text using the caret symbol (`^`), but that is not the exponent operator in Python.

```python
5^3
# 53
```

In Python, `^` means bitwise XOR, so `5^3` evaluates to `53` rather than `125`.
