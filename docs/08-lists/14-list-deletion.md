# List Deletion

Python has a built-in keyword, `del`, that deletes items from objects. With lists, you can use it to delete a single item or an entire slice.

```python
nums = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# Delete the fourth item
del nums[3]
print(nums)
# Output: [1, 2, 3, 5, 6, 7, 8, 9]
```

You can also delete a range of items:

```python
nums = [1, 2, 3, 4, 5, 6, 7, 8, 9]

# Delete the second item up to (but not including) the fourth item
del nums[1:3]
print(nums)
# Output: [1, 4, 5, 6, 7, 8, 9]
```

To clear a list completely, delete the full slice:

```python
nums = [1, 2, 3, 4, 5, 6, 7, 8, 9]

del nums[:]
print(nums)
# Output: []
```