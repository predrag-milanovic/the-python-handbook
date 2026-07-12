# Counting the Items in a List

Remember that we can [iterate](https://en.wikipedia.org/wiki/Iteration) over all the elements in a list using a loop. One common pattern is to loop over the indexes in the list with `range()` and `len()`.

```python
sports = ["soccer", "basketball", "tennis", "swimming"]

for i in range(0, len(sports)):
	print(sports[i])
```

This prints each item in the `sports` list one by one.
