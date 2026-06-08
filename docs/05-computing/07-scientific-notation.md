# Scientific Notation

As we covered earlier, a `float` is a positive or negative number with a fractional part.

You can add the letter `e` or `E` followed by a positive or negative integer to use [scientific notation](https://en.wikipedia.org/wiki/Scientific_notation):

```python
print(16e3)
# Prints 16000.0

print(7.1e-2)
# Prints 0.071
```

If you are not familiar with scientific notation, it is a way to write numbers that are too large or too small to conveniently write out in full.

In short, the exponent after the `e` tells Python how many places to move the decimal point. A positive exponent moves it to the right, and a negative exponent moves it to the left.

## Underscores for Readability

Python also lets you use underscores as the [delimiter](https://en.wikipedia.org/wiki/Decimal_separator#Digit_grouping) instead of commas to make large decimal numbers easier to read:

```python
num = 16_000
print(num)
# Prints 16000

num = 16_000_000
print(num)
# Prints 16000000
```
