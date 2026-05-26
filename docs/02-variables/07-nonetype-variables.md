# NoneType Variables

Not every variable starts with a value. We can create an "empty" variable by setting it to [`None`](https://docs.python.org/3/library/constants.html#None).

`None` is a special value in Python that represents the absence of a value. It is not the same as zero, `False`, or an empty string.

One common use case is when a value has not been determined yet. For example, you might wait for a user to enter their name:

```python
username = None
```

Later, once the user gives you input, you can assign it to the variable:

```python
username = input("What's your name? ")
```

In this case, `username` starts as `None` until we use the assignment operator, `=`, to give it a value.

## None Is Not a String

[`NoneType`](https://docs.python.org/3/library/types.html#types.NoneType) is not the same as a string with the value `"None"`:

```python
str_none = "None"
actual_none = None

print(str_none)  # None
print(actual_none)  # None

print(type(str_none))  # <class 'str'>
print(type(actual_none))  # <class 'NoneType'>
```

That difference matters because Python treats the two values differently, even though they look similar when printed.

If you use `"None"` instead of `None`, your code may look correct in the console but still fail tests that check the actual data type.
