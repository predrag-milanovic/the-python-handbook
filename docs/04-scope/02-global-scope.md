# Global scope

So far we've been working in the global scope. That means names (variables and functions) defined at the top level of a module are accessible throughout that module — including inside other functions.

Example:

```python
pi = 3.14

def get_area_of_circle(radius):
	return pi * radius * radius
```

Because `pi` was declared in the parent "global" scope, it is usable within `get_area_of_circle()`.
