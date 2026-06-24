# Loops

Loops let us run the same piece of code multiple times without writing it again and again. They're essential when you need to repeat an operation, whether that's 10 times, 1,000 times, or 1,000,000 times.

Python has two main loop types:

- `for` loops, which iterate over a sequence (like `range()`, a list, or a string)
- `while` loops, which continue as long as a condition stays `True`

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

## While

Python has another type of loop, the `while` loop. It's a loop that continues `while` a condition remains `True`.

The syntax is simple:

```python
while 1:
    print("1 evaluates to True")

# prints:
# 1 evaluates to True
# 1 evaluates to True
# (...continuing)
```

The example above is hardcoded to continue forever, creating an infinite loop.

Typically, a `while` loop condition is a comparison or variable, and it determines when the loop ends:

```python
num = 0
while num < 3:
    num += 1
    print(num)

# prints:
# 1
# 2
# 3
# (the loop stops when num >= 3)
```

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

