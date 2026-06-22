# Loops

Loops let us run the same piece of code multiple times without writing it again and again. They're essential when you need to repeat an operation — whether 10 times, 1,000 times, or 1,000,000 times.

For example, if we wanted to print the numbers 0 through 9 you could write nine `print()` calls manually:

```python
print(0)
print(1)
print(2)
print(3)
print(4)
print(5)
print(6)
print(7)
print(8)
print(9)
```

That's tedious and error-prone. A `for` loop does the same work clearly and concisely:

```python
for i in range(0, 10):
	print(i)
```

Here `i` is a loop variable that takes each value from `range(0, 10)` in turn. The loop runs the indented block (the loop body) once per value of `i`.

## How `range()` works

- `range(start, stop)` produces values starting at `start` and ending *before* `stop` (stop is exclusive).
- `range(stop)` is the same as `range(0, stop)`.
- `range(start, stop, step)` lets you change the step (defaults to `1`). A negative `step` iterates in reverse.

Examples:

```python
list(range(5))        # [0, 1, 2, 3, 4]
list(range(0, 10, 2)) # [0, 2, 4, 6, 8]
list(range(10, 0, -1))# [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]
```

## Whitespace matters

Python uses indentation to group code. The body of a `for` loop must be indented. Forgetting to indent the loop body raises a `SyntaxError`:

```python
for i in range(3):
print(i)  # SyntaxError: expected an indented block
```

Always use a consistent indentation style (4 spaces is the common convention).

## Step-by-step (what the `for` loop does)

For `for i in range(0, 10):` the loop does roughly this:

1. Set `i = 0` (the first value from `range`).
2. Check whether there is a value available; if not, exit the loop.
3. Execute the body (`print(i)`).
4. Move to the next value of `i` (1), then go back to step 2.

This prints the numbers `0` through `9` in order.
