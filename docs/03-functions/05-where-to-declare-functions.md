Where to Declare Functions

You've probably noticed that a variable must be created before it's used. For example, this raises an error:

```python
print(my_name)
my_name = 'Predrag Milanovic'
# NameError: name 'my_name' is not defined
```

It needs to be written in the other order:

```python
my_name = 'Predrag Milanovic'
print(my_name)
# Predrag Milanovic
```

Code executes in order from top to bottom. That means a name (variable or function) must exist before the code that uses it runs.

Functions follow the same rule: you cannot call a function at runtime before it has been defined. A common source of confusion is the difference between the order of definitions in the file and the order in which code actually runs. The important rule is: at the moment your program tries to call a function, that function's `def` must already have been executed.

Example — incorrect order:

```python
greet()

def greet():
	print("hello")

# NameError: name 'greet' is not defined (because the call happens before the def)
```

Example — correct order:

```python
def greet():
	print("hello")

greet()  # prints "hello"
```

Note: it's fine for a function to call another function that is defined later in the file, as long as the call doesn't happen until after both functions have been defined (for example, if the call occurs at runtime inside a different function). The runtime order, not the textual order alone, determines whether a name is available.

Keep this simple rule in mind when organizing your code: ensure definitions exist before you use them at runtime.

