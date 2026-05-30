# None Return

When a function does not explicitly return a value, Python automatically returns `None`.

This commonly happens for functions that perform an action (for example, printing) but do not produce a value for the caller to use. The three snippets below all behave the same: they return `None` when called.

```python
def my_func():
	print("I do nothing")
	return None

def my_func():
	print("I do nothing")
	return

def my_func():
	print("I do nothing")
```

In all three cases, calling `my_func()` will print "I do nothing" and the expression `my_func()` evaluates to `None`.

If you accidentally forget to `return` a value from a function that should produce one, the `None` value can lead to bugs later — for example, trying to use the result in arithmetic or string formatting will raise errors. Use `return` when callers need a value; use implicit `None` (or `return` with no value) only when the function's purpose is its side effects.

