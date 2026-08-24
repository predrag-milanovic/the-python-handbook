# Tuple Hints

[Lists](https://docs.python.org/3/library/stdtypes.html#lists) and [sets](https://docs.python.org/3/library/stdtypes.html#set-types-set-frozenset) usually hold multiple values of the same type. For example:

```python
inventory: list[str] = ["Black Knight Halberd", "Skull Lantern", "Notched Whip"]
```

[Tuples](https://docs.python.org/3/library/stdtypes.html#tuples), on the other hand, are small, fixed groups of values. Each position has its own meaning, so the values often have different types. For example, a loot drop might contain an item name and a quantity:

```python
drop: tuple[str, int] = ("Garnet Mark", 2)
```

The type hint `tuple[str, int]` means:

- the tuple contains two values
- the first value is a string
- the second value is an integer

A tuple can contain any number of values, although two- and three-value tuples are common. For example, these values represent a character's HP, MP, and stamina:

```python
stats: tuple[int, float, int] = (100, 42.5, 75)
```

The type hint `tuple[int, float, int]` describes a three-value tuple containing an integer, a float, and another integer. As with other type hints, it describes the intended types but does not prevent different values from being added at runtime.
