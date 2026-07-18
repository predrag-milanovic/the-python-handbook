# Tuples

[Tuples](https://docs.python.org/3/library/stdtypes.html#typesseq-tuple) are collections of data that are ordered and unchangeable.

You can think of a tuple as a list with a fixed size. Tuples are created with round brackets:

```python
my_tuple = ("this is a tuple", 45, True)

print(my_tuple[0])
# this is a tuple
print(my_tuple[1])
# 45
print(my_tuple[2])
# True
```

It is usually a bad idea to store different types of data in a list, but that is not a problem for tuples. Because tuples have a fixed size, it is easier to keep track of which index stores which type of value.

Tuples are often used for very small groups of related data, like a dog's name and age:

```python
dog = ("Fido", 4)
```

There is a special case for single-item tuples. You must include a comma so Python knows it is a tuple and not just regular parentheses:

```python
dog = ("Fido",)
```

Because tuples can be stored in lists, you can build a list of tuples. The first index selects which tuple you want, and the second index selects a value inside that tuple:

```python
my_tuples = [
    ("this is the first tuple in the list", 45, True),
    ("this is the second tuple in the list", 21, False),
]

print(my_tuples[0][0])
# this is the first tuple in the list
print(my_tuples[0][1])
# 45
print(my_tuples[1][0])
# this is the second tuple in the list
print(my_tuples[1][2])
# False
```

## Tuple Unpacking

You can assign the values of a tuple to separate variables with unpacking:

```python
dog = ("Fido", 4)
dog_name, dog_age = dog

print(dog_name)
# Fido
print(dog_age)
# 4
```

When you return multiple values from a function, Python is actually returning a tuple.
