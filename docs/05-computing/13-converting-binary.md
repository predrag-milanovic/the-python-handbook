# Converting Binary

Binary strings represent numbers in base 2 (each digit is 0 or 1). Examples:

- "100" -> 4
- "101" -> 5
- "10010" -> 18

The built-in [int()](https://docs.python.org/3/library/functions.html#int) function can convert a binary string to an integer by passing the base (2) as the second argument:

```python
# this is a binary string
binary_string = "100"

# convert binary string to integer
num = int(binary_string, 2)
print(num)
# 4
```

Notes:

- If the string contains characters other than `0` or `1` (after optional whitespace), `int()` will raise a `ValueError`.
- If the string includes the `0b` prefix (for example `"0b100"`), you can use `int(s, 0)` to let Python infer the base from the prefix.

That's all you need to convert binary strings to integers in Python.

