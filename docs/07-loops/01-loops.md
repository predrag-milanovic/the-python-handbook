# Loops

Loops let us run the same piece of code multiple times without writing it again and again. They're essential when you need to repeat an operation, whether that's 10 times, 1,000 times, or 1,000,000 times.

As a reminder, a `for` loop in Python is written like this:

```python
for i in range(0, 10):
    print(i)
```

In English, the code says:

1. Start with `i` equal to `0`.
2. If `i` is greater than or equal to `10`, exit the loop.
3. Print `i` to the console.
4. Add `1` to `i`.
5. Go back to step 2.

The result is that the numbers `0` through `9` are logged to the console in order.

## How `range()` works

The `range()` function creates a sequence of numbers for the loop to iterate over.

- `range(start, stop)` produces values starting at `start` and ending *before* `stop` (stop is exclusive).
- `range(stop)` is the same as `range(0, stop)`.
- `range(start, stop, step)` lets you change the step (defaults to `1`). A negative `step` iterates in reverse.

Examples:

```python
list(range(5))        # [0, 1, 2, 3, 4]
list(range(0, 10, 2)) # [0, 2, 4, 6, 8]
list(range(10, 0, -1)) # [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]
```

## Whitespace Matters in Python!

Python uses indentation to group code. The body of a `for` loop *must* be indented; otherwise, you'll get a syntax error:

```python
for i in range(3):
print(i)  # SyntaxError: expected an indented block
```

Always use a consistent indentation style. Four spaces is the common convention.

## Assignment

In the `print_numbers` function, write a `for` loop from scratch that logs the numbers `0` through `199` to the console.

```python
def print_numbers():
    pass
```

Don't edit the code below this line.
