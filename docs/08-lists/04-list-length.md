# List Length

The length of a list can be calculated with the `len()` function. It takes an iterable, such as a list or string, and returns the number of items it contains.

```python
fruits = ["apple", "banana", "pear"]
length = len(fruits)

print(length)
# 3

print(len("supercalifragilisticexpialidocious"))
# 34
```

Don't confuse the length of a list with the index of its last item. Since indexes start at `0`, the last index is always one less than the length.

```python
fruits = ["apple", "banana", "pear"]

print(len(fruits))
# 3

print(fruits[2])
# pear
```
