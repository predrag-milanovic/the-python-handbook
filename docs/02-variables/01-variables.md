# Variables

[Variables](https://users.cs.utah.edu/~germain/PPS/Topics/variables.html) are how we store data as our program runs. Until now, we've been passing values straight into [`print()`](https://docs.python.org/3/library/functions.html#print). With variables, we can save a value, reuse it later, and change it before printing it.

## Creating variables

A variable is just a name we give to a value. For example, we can create a variable named `my_height` and set it to `100`:

```python
my_height = 100
```

We can also create a variable named `my_name` and set it to the text string `"Predrag"`:

```python
my_name = "Predrag"
```

You can choose almost any name for a variable, but good variable names are descriptive and usually written as a single [token](https://en.wikipedia.org/wiki/Lexical_analysis#Token) with underscores between words.

## Using variables

Once a variable exists, we can use its name to access the value it stores. This prints `100`:

```python
print(my_height)
```

And this prints `Lane`:

```python
print(my_name)
```

The main benefit is that the value lives in one place. If you need to use it more than once, a variable keeps your code cleaner and easier to update.

# Variables Vary

Variables are called variables because the value they hold can change. In other words, the value varies over time.

For example, this code prints `20`:

```python
acceleration = 10
acceleration = 20
print(acceleration)
```

The line `acceleration = 20` reassigns `acceleration` to `20`. It overwrites the previous value, which was `10`.
