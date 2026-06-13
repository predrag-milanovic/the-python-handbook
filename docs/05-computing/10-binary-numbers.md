# Binary Numbers

[Binary numbers](https://en.wikipedia.org/wiki/Binary_number) are just base 2 numbers. They work the same way as base 10 numbers, but binary uses two symbols instead of ten.

- Base 2 symbols: `0` and `1`
- Base 10 symbols: `0`, `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9`

Each digit's place value is double the place to its right. In a 4-digit binary number, the place values are:

```text
Binary digits:   0   1   0   1
Place values:    8   4   2   1
```

For example, `0101` means:

- `0` eights
- `1` four
- `0` twos
- `1` one

So `0101` is `5` in decimal:

```text
0 x 8 + 1 x 4 + 0 x 2 + 1 x 1 = 5
```

## Binary in Python

You can write an integer in Python using binary syntax with the `0b` prefix:

```python
print(0b0001)
# Prints 1

print(0b0101)
# Prints 5
```

Leading zeros are often added for visual consistency, but they do not change the value of a binary number.

## Quick Check

What does the binary number `1100` represent in decimal?

- `1`
- `8`
- `2`
- `15`
- `3`
- `13`
- `4`
- `12`
