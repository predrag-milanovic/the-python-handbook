# Dictionary Hints

[Dictionaries](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict) are container types too, but they map **keys** to **values**. Because a dictionary contains two kinds of values, its type hint includes both types:

```python
item_counts: dict[str, int] = {
	"Wooden Arrow": 30,
	"Small Amethyst": 2,
}
```

The first type is the type of the keys, and the second type is the type of the values:

```python
dict[key_type, value_type]
```

So `dict[str, int]` means:

- the keys are strings
- the values are integers

Dictionary keys must be [hashable](https://docs.python.org/3/glossary.html#term-hashable). The key types you'll see most often are strings and integers. Dictionary values, on the other hand, can be any type.

As with other type hints, `dict[str, int]` describes the intended types but does not prevent a program from adding a value of another type at runtime.
