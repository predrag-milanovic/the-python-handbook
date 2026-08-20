# List and Set Hints

We've covered hints for **basic types** like `str`, `int`, `float`, and `bool`, but you can also add hints for **container types**: types that *hold other values*. For example:

- [`list`](https://docs.python.org/3/library/stdtypes.html#lists): mutable sequence of values
- [`set`](https://docs.python.org/3/library/stdtypes.html#set-types-set-frozenset): unordered collection of unique values
- [`dict`](https://docs.python.org/3/library/stdtypes.html#mapping-types-dict): collection of key-value pairs
- [`tuple`](https://docs.python.org/3/library/stdtypes.html#tuples): immutable sequence of values

When we type-hint a container, we specify both what kind of container it is and what type of values it contains. For example, a *list* of *strings* can be expressed as `list[str]`:

```python
inventory: list[str] = ["Iron Sword", "Healing Potion"]
```

The contained type goes in square brackets after the container type. Similarly, for a *set* of *strings*, we write `set[str]`:

```python
unique_items: set[str] = {"Iron Sword", "Healing Potion"}
```

These built-in generic types use the square-bracket syntax introduced in Python 3.9. The type hint describes the intended contents; it does not prevent a program from adding a value of another type at runtime.
