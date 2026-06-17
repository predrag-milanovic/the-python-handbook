# If-Else

An `if` statement can be followed by zero or more `elif` statements, which can be followed by zero or one `else` statement.

`elif` stands for "else if". It gives you another condition to check when the earlier ones are `False`.

For example:

```python
if score > high_score:
	print("High score beat!")
elif score > second_highest_score:
	print("You got second place!")
elif score > third_highest_score:
	print("You got third place!")
else:
	print("Better luck next time")
```

First the `if` statement is evaluated. If it is `True`, then the if statement's body is executed and all the other `elif` statements and the `else` statement are ignored.

If the first `if` is `False`, then the next `elif` is evaluated. Likewise, if it is `True`, then its body is executed and the rest are ignored.

If none of the `if` or `elif` statements evaluate to `True`, then the final `else` statement is the only body executed.

If-Else Practice

Here are some basic rules with `if` / `else` blocks.

- You can't have an `elif` or an `else` without an `if`
- You *can* have an `else` without an `elif`

Remember, to check if two values are the same use the `==` operator.

```python
are_equal = 5 == 6
# are_equal is False

are_equal = 6 == 6
# are_equal is True
```
