# Errors and Exceptions in Python

You've probably seen a few errors by now. In Python, the two main kinds you'll run into are:

- Syntax errors
- Exceptions

## Syntax Errors

A syntax error means the Python interpreter couldn't even understand the code because it doesn't follow Python's rules.

```python
this is not valid code, so it will error
```

If we try to run that sentence as code, Python raises a syntax error:

```python
this is not valid code, so it will error
	  ^
SyntaxError: invalid syntax
```

## Exceptions

Even when code has valid syntax, it can still fail while it is running. Errors that happen during execution are called exceptions.

Exceptions can be handled so your program doesn't crash immediately. Python uses a `try` / `except` block for that:

```python
try:
	10 / 0
except Exception:
	print("can't divide by zero")
```

Here's how that works:

The code inside `try` runs until it finishes or an exception is raised.
If an exception happens, Python jumps to the matching `except` block.
If no exception happens, the `except` block is skipped.

If we want the exception message itself, we can save it with `as`:

```python
try:
	10 / 0
except Exception as e:
	print(e)

# division by zero
```

Using `try` / `except` lets us handle failures gracefully instead of crashing the whole program.
