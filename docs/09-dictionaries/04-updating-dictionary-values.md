# Updating Dictionary Values

If you assign a new value to a key that already exists, Python updates the value for that key instead of creating a new one.

```python
planets = {
	"Pluto": True,
}

planets["Pluto"] = False

print(planets["Pluto"])
# Prints: False
```

This works the same way for any existing key in the dictionary.
