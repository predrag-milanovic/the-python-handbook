# Iterating Over a Dictionary in Python

We can iterate over a dictionary's keys using the same no-index syntax we used to iterate over the values in a list. Once we have each key, we can use it to access the key's corresponding value.

```python
fruit_sizes = {
	"apple": "small",
	"banana": "large",
	"grape": "tiny",
}

for name in fruit_sizes:
	size = fruit_sizes[name]
	print(f"name: {name}, size: {size}")

# name: apple, size: small
# name: banana, size: large
# name: grape, size: tiny
```

We could have just as easily set the `name` variable to `key` or simply `k`.
