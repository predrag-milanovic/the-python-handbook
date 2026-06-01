# Default Values

In Python, you can give a function parameter a [default](https://docs.python.org/3/glossary.html#term-parameter) value. This is useful when a parameter is optional and the caller does not always need to provide it.

A default value is created with the assignment operator (`=`) in the function signature.

```python
def get_greeting(email, name="there"):
	print("Hello", name, "welcome! You've registered your email:", email)
```

```python
get_greeting("predrag@example.com", "Predrag")
# Hello Predrag welcome! You've registered your email: predrag@example.com
```

```python
get_greeting("predrag@example.com")
# Hello there welcome! You've registered your email: predrag@example.com
```

If the second parameter is omitted, Python uses the default `"there"` value instead.

For this to work, parameters with default values must come after all required parameters in the function definition.
