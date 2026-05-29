# Multiple Parameters

Functions can have more than one parameter. A parameter is a named input that a function receives.

Here is a simple example:

```python
def subtract(a, b):
	result = a - b
	return result
```

When a function has multiple parameters, the position of each argument matters. The first argument goes to the first parameter, the second argument goes to the second parameter, and so on.

This function is called with `5` for `a` and `3` for `b`:

```python
result = subtract(5, 3)
print(result)
# 2
```

If we change the order of the arguments, the result changes too.

Here is a larger example with four parameters:

```python
def create_introduction(name, age, height, weight):
	first_part = "Your name is " + name + " and you are " + age + " years old."
	second_part = "You are " + height + " meters tall and weigh " + weight + " kilograms."
	full_intro = first_part + " " + second_part
	return full_intro
```

We can call it like this:

```python
my_name = "John"
my_age = "30"

intro = create_introduction(my_name, my_age, "1.8", "80")
print(intro)
# Your name is John and you are 30 years old. You are 1.8 meters tall and weigh 80 kilograms.
```

In this example, `my_name` is passed to `name`, `my_age` is passed to `age`, `"1.8"` is passed to `height`, and `"80"` is passed to `weight`.

When you use multiple parameters, keep the order clear and consistent so the function gets the right values.
