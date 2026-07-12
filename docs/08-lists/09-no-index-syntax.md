# No-Index Syntax

Python makes it easy to iterate directly over the items in a list without dealing with index numbers. If you do not need the index, this is often the cleanest way to write the loop.

```python
trees = ["oak", "pine", "maple"]

for tree in trees:
	print(tree)

# Prints:
# oak
# pine
# maple
```

The variable after `for` - in this example, `tree` - refers to each value in the list, not its index. When you only need the item itself, this syntax is simpler and easier to read than looping over indexes.
