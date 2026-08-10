# Function Parameters

[Function parameters](https://docs.python.org/3/glossary.html#term-parameter) can have type hints too. The syntax is the same as variable type hints: put a colon after the parameter name, then the type.

```python
def greet_player(name: str):
    print(f"Welcome, {name}!")
```

When a function has multiple parameters, each one can have its own type hint:

```python
def add_gold(current_gold: int, found_gold: int):
    return current_gold + found_gold
```

A type hint on a simple variable assignment can feel a little redundant because Python can often infer the type from the value:

```python
character_health: float = 72.5
```

Function parameters are different. If you do not add hints, your editor will not know what kinds of values the function expects, so autocomplete and error checking will be less useful.

If your editor supports it, hovering over a variable can show its type. In this example, `status` might appear as a string. The parameters `name`, `level`, `health`, and `has_magic` would stay "unknown" unless you add type hints.

```python
def build_status(name, level, health, has_magic):
    status = f"{name} is level {level}"
    return status
```
