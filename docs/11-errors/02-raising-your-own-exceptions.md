# Raising Your Own Exceptions

Errors are not something to be scared of. In a real program, errors are part of normal control flow, and our job is to handle them in a way that matches the user's expectations.

## Errors Are Not Bugs

When our own code reaches a state that should not happen, we can raise an exception on purpose.

That does not automatically mean there is a bug. A bug is when the program behaves in a way the user did not expect. Raising an exception can be the correct way to stop an invalid action before it causes worse problems.

For example, imagine a game where players can craft swords from only a few valid materials:

```python
def craft_sword(metal_bar):
	if metal_bar == "bronze":
		return "bronze sword"
	if metal_bar == "iron":
		return "iron sword"
	if metal_bar == "steel":
		return "steel sword"

	raise Exception("invalid metal bar")
```

If someone tries to craft a sword from a material that is not supported, `raise` stops the function immediately and forces the problem to be handled.

## Don't Catch Your Own Exceptions

As a rule, do not raise an exception and then catch it in the same function just to print a message.

```python
# don't do this
def craft_sword(metal_bar):
	try:
		if metal_bar == "bronze":
			return "bronze sword"
		if metal_bar == "iron":
			return "iron sword"
		if metal_bar == "steel":
			return "steel sword"

		raise Exception("invalid metal bar")
	except Exception as e:
		print(f"An error occurred: {e}")
```

Instead, let the caller decide what to do with the error:

```python
try:
	craft_sword("gold bar")
except Exception as e:
	print(e)

# invalid metal bar
```

This keeps `craft_sword` focused on one job: validating the input and raising an exception when the input is not allowed. The caller can then decide whether to log the error, show a message, or stop the program completely.
