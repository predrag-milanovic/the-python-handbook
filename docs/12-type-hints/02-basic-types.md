# Basic Types

To add a type hint to a variable declaration, put a colon after the variable name, then the type. This comes before the equals sign and the value:

```python
character_name: str = "Sir Galahad"
character_level: int = 7
character_health: float = 72.5
has_magic: bool = True
```

The values work the same way they did before. The type hint does not change how the variable behaves.

For simple assignments like this, you do not actually need the hint. Python can usually infer the type from the value:

```python
character_health = 72.5
```

Because `character_health` is assigned `72.5`, your editor can infer that it is a `float`. If you want the type name to be visible, you can still add the hint:

```python
character_health: float = 72.5
```

That is the basic pattern for variable type hints: name, colon, type, equals sign, value.
