# Changing in Place

It is common to change the value of a variable based on its current value.

```python
player_score = 4
player_score = player_score + 1
# player_score now equals 5
```

```python
player_score = 4
player_score = player_score - 1
# player_score now equals 3
```

The expression `player_score = player_score - 1` may look strange if you read it like a math equation, but it is valid code.

Read it as:

> Assign to `player_score` the current value of `player_score` minus 1.

Python evaluates the right-hand side first. Once it has the result, it updates `player_score` with the new value.
