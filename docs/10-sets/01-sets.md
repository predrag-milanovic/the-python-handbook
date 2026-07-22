# Sets

Sets are like lists, but they are unordered and guarantee uniqueness. Only one of each value can be in a set.

```python
fruits = {"apple", "banana", "grape"}
print(type(fruits))
# Prints: <class 'set'>

print(fruits)
# Prints: {'banana', 'grape', 'apple'}
```

## Add Values

You can add values to a set with `.add()`. Think of `.add()` like `append()`, but for sets.

```python
fruits = {"apple", "banana", "grape"}
fruits.add("pear")
print(fruits)
# Prints: {'pear', 'banana', 'grape', 'apple'}
```

If you add a value that is already in the set, nothing changes and no error is raised.

## An Empty Set

The `{}` syntax creates an empty dictionary, not an empty set. To create an empty set, use the `set()` function.

```python
fruits = set()
fruits.add("pear")
print(fruits)
# Prints: {'pear'}
```

## Set Iteration

```python
fruits = {"apple", "banana", "grape"}

for fruit in fruits:
	print(fruit)
	# Prints:
	# banana
	# grape
	# apple
```

Sets are unordered, so the order of iteration is not guaranteed.
