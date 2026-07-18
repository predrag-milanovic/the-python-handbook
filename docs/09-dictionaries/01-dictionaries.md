# Dictionaries

[Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries) in Python are used to store data values in key-value pairs. They are a good way to store groups of information.

You can create a dictionary with curly braces `{}` and add key-value pairs inside it:

```python
# use curly braces
# add key-value pairs
car = {
	"brand": "Toyota",
	"model": "Camry",
	"year": 2019,
}

print(car["brand"])
# Toyota
print(car["model"])
# Camry
print(car["year"])
# 2019
```

Here, the `car` variable is assigned to a dictionary containing the keys `brand`, `model`, and `year`. The keys' corresponding values are `Toyota`, `Camry`, and `2019`.

## Duplicate Keys

Dictionary keys must be unique. If you use the same key more than once in the same dictionary, the later value replaces the earlier one.