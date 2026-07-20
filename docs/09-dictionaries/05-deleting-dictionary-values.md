# Deleting Dictionary Values

You can delete an existing key from a dictionary with the `del` keyword.

```python
names_dict = {
	"jack": "bronson",
	"jill": "mcarty",
	"joe": "denver",
}

del names_dict["joe"]

print(names_dict)
# Prints: {'jack': 'bronson', 'jill': 'mcarty'}
```

## Deleting Keys That Don't Exist

If you try to delete a key that is not in the dictionary, Python raises an error.

```python
names_dict = {
	"jack": "bronson",
	"jill": "mcarty",
	"joe": "denver",
}

del names_dict["unknown"]
# Raises a KeyError because the key does not exist
```
