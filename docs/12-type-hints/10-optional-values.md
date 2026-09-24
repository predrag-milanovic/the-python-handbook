# Optional Values

Sometimes a variable may or may not have an actual value. For example, a character might have a damage bonus, or they might not. When there is no value, we can represent that with `None`.

The `|` operator means a value can be one of several types:

```python
damage_bonus: int | None
```

Here, `damage_bonus` is either an integer (the bonus amount) or `None` (no bonus).

## Optional return values

Functions can return optional values too. For example, a function might return a prepared spell if one is ready, or `None` if no spell is prepared:

```python
def get_prepared_spell(has_spell: bool) -> str | None:
    if has_spell:
        return "Fireball"

    return None
```

The `-> str | None` part means the function returns either a string or `None`.

## Checking for `None`

Because an optional value might be `None`, check it before you use it:

```python
spell = get_prepared_spell(True)

if spell is not None:
    print(f"Casting {spell}!")
else:
    print("No spell is prepared.")
```

Use `is` and `is not` to compare with `None`, not `==` and `!=`.

## The older `Optional` syntax

In older code, you may see the same idea written with `Optional` from the `typing` module:

```python
from typing import Optional

damage_bonus: Optional[int]
```

`Optional[int]` means the same thing as `int | None`. The `|` syntax works in Python 3.10 and later, and it is the style this handbook uses.
