# Return Types

You can also annotate the type that a function is expected to return. When you know what kinds of values go into a function and what kind of value comes out, you can often understand the function without reading every line of its body.

Return types come after the parameter list and before the colon:

```python
def add_gold(current_gold: int, found_gold: int) -> int:
    return current_gold + found_gold
```

The `-> int` part means this function is expected to return an integer.

The syntax is a little different from type hints on variables and parameters:

- we use `->` instead of `:`
- there is no variable name before the type hint

This is because it does not matter what name the function uses internally for the return value. We care about the type, not the local name.

Here is another example:

```python
def get_greeting(player_name: str) -> str:
    return f"Welcome, {player_name}!"
```

The `-> str` part means this function is expected to return a string.
