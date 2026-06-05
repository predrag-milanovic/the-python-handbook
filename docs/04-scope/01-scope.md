# Scope

Scope refers to *where* a variable or function name is available to be used. When we create variables inside a function (for example, parameter names or local variables), that data is *not* available outside the function.

## Example

```python
def subtract(x, y):
	return x - y

result = subtract(5, 3)
print(x)
# ERROR! "name 'x' is not defined"
```

When the `subtract` function is called, `x` is assigned the value `5`, but `x` only exists inside the `subtract` function.

If we try to access `x` from outside the function we get a `NameError` because the variable is out of scope.
