# Set Subtraction

You can use some of the normal mathematical operations on sets. For example, you can subtract one set from another.

Set subtraction removes every value in the second set from the first set and returns a new set with the remaining values.

```python
set1 = {"apple", "banana", "grape"}
set2 = {"apple", "banana"}
set3 = set1 - set2

print(set3)
# Prints: {'grape'}
```
