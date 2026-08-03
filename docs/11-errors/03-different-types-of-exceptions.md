# Different Types of Exceptions

We have not covered classes and objects yet, which is what an `Exception` really is at its core. We will go into that later in the course on object-oriented programming.

For now, the important idea is that there are different types of exceptions, and we can handle them differently depending on the situation.

Some exceptions are very specific, like `ZeroDivisionError`, which happens when you divide by zero, or `IndexError`, which happens when you try to access a list item at an invalid index. Other exceptions are more general, like the base `Exception`.

## Syntax

You can catch specific exceptions first, and then fall back to a more general one:

```python
try:
	10 / 0
except ZeroDivisionError:
	print("0 division")
except Exception as e:
	print(e)

try:
	nums = [0, 1]
	print(nums[2])
except IndexError:
	print("index error")
except Exception as e:
	print(e)

# 0 division
# index error
```

## Why Specific Exceptions Come First

When handling exceptions, it is important to catch the most specific ones first, because Python stops checking once it finds a matching handler.

If you catch a more general `Exception` first, any specific errors below it will never be reached:

```python
try:
	nums = [0, 1]
	print(nums[2])
except Exception:
	print("An error occurred")
except IndexError:
	print("Index error")

# An error occurred
```

In this example, the general `Exception` catches the error before the `IndexError` handler can run.

Always handle the most specific exception first.

## Using `as`

You can also save the exception with `as` and then print the error message itself:

```python
try:
	10 / 0
except Exception as e:
	print(e)

# division by zero
```

The `print` function prints the string representation of whatever object is passed to it. In this case, that means it prints the error message.
