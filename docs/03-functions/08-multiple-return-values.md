# Multiple Return Values

A function can return more than one value by separating them with commas.

```python
def cast_iceblast(wizard_level, start_mana):
	damage = wizard_level * 2
	new_mana = start_mana - 10
	return damage, new_mana  # return two values
```

## Receiving Multiple Values

When you call a function that returns multiple values, you can assign them to multiple variables.

```python
damage, mana = cast_iceblast(5, 100)
print(f"Damage: {damage}, Remaining Mana: {mana}")
# Damage: 10, Remaining Mana: 90
```

When `cast_iceblast` is called, it returns two values. The first value is assigned to `damage`, and the second value is assigned to `mana`.

Just like with function inputs, order matters. The variable names do not affect which value is assigned first.

We could just as easily have used different variable names:

```python
one, two = cast_iceblast(5, 100)
print(f"Damage: {one}, Remaining Mana: {two}")
# Damage: 10, Remaining Mana: 90
```

Descriptive variable names make code easier to understand, so choose them carefully.

## What Happened to the Variables?

The `damage` and `new_mana` variables inside `cast_iceblast` only exist inside that function.

They cannot be used outside of the function body. We will talk more about this when we cover scope.
