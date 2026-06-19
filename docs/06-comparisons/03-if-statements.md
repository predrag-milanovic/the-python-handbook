# If Statements

It is often useful to run code only when a condition is met. In Python, an `if` statement lets you do that.

```python
if CONDITION:
	# do some stuff here

# code after the if block may still run regardless
```

The body of the `if` statement only runs when the condition is `True`. Code after the `if` block still runs unless something stops the function first.

Example

```python
def show_status(boss_health):
	if boss_health > 0:
		print("Ganondorf is alive!")
		return

	print("Ganondorf is unalive!")
```

If `boss_health` is greater than `0`, this function prints:

```text
Ganondorf is alive!
```

Otherwise, it prints:

```text
Ganondorf is unalive!
```

Without the `return` inside the `if` block, the second message would always run:

```python
def show_status(boss_health):
	if boss_health > 0:
		print("Ganondorf is alive!")

	print("Ganondorf is unalive!")
```

That version could print both messages:

```text
Ganondorf is alive!
Ganondorf is unalive!
```

When you want code in an `if` block to stop the rest of a function from running, use `return` to exit early.

Two syntax details matter here:

- Indentation tells Python where the `if` block ends.
- The colon after `if CONDITION` is required.

If Practice

Remember, you can use the `==` operator to check whether two values are equal.

```python
is_equal = 5 == 5
# is_equal is True
```
