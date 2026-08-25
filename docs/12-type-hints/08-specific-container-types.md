# Specific Container Types

You can type-hint a container with just its container type. For example:

```python
items: list = ["Black Firebomb", "Titanite Chunk"]
```

This tells us that `items` is a [list](https://docs.python.org/3/library/stdtypes.html#lists), but it does not tell us what kind of values the list contains. When you know the value type, be more specific:

```python
items: list[str] = ["Black Firebomb", "Titanite Chunk"]
```

The type hint `list[str]` means that the list is intended to contain strings.

Bare container hints are not always wrong. Sometimes you do not know what types of values a container will hold, or a more specific hint would be too complicated to be useful. You may occasionally see this with [dictionaries](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict). Give clear, specific type hints whenever possible.
