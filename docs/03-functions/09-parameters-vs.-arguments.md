# Parameters vs. Arguments

Parameters are the names used for inputs when *defining* a function. Arguments are the values passed into a function when it is *called*.

To put it another way, arguments are the actual values, such as `42.0`, `"the dark knight"`, or `True`.

Parameters are the names we use in the function definition to refer to those values. When we write the function, those names can be anything we choose.

```python
# a and b are parameters
def add(a, b):
	return a + b

# 5 and 6 are arguments
sum = add(5, 6)
```

In the example above, `a` and `b` are the parameters because they appear in the function definition.

The values `5` and `6` are the arguments because they are the values passed into the function call.

This distinction is useful, but developers often use the words interchangeably in conversation. If you hear someone say “arguments” when they mean “parameters,” they are usually talking about the same basic idea.
