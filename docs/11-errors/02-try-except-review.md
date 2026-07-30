# Try/Except Review

```python
try:
	10 / 0
except Exception as e:
	print(e)

# prints "division by zero"
```

The `try` block runs until an exception is raised or it finishes, whichever comes first. In this example, Python raises a `ZeroDivisionError` because dividing by zero is impossible.

The `except` block runs only when an exception is raised in the `try` block. It also gives you the exception as data (`e` here), so you can handle the problem gracefully instead of crashing the program.
