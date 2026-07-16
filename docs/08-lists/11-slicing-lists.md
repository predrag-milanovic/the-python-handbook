# Slicing Lists

Python makes it easy to work with only part of a list. To do that, use slice syntax with a colon `:`.

List slicing returns a new list from the original list. You can control where the slice starts, where it stops, and how many items it skips each time.

```python
my_list[start:stop:step]
```

The `start` index is included, but the `stop` index is not. All three parts are optional.

```python
scores = [50, 70, 30, 20, 90, 10, 50]

print(scores[1:5:2])
# Prints [70, 20]
```

In that example, the slice starts at index `1`, stops before index `5`, and takes every second item.

## Omitting Sections

You do not always need all three parts of the slice.

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

print(numbers[:3])
# Prints [0, 1, 2]

print(numbers[3:])
# Prints [3, 4, 5, 6, 7, 8, 9]
```

If you leave out `start`, Python starts at the beginning of the list. If you leave out `stop`, Python goes to the end.

## Using Only the Step

You can also leave out both `start` and `stop` and only provide a step.

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

print(numbers[::2])
# Prints [0, 2, 4, 6, 8]
```

## Negative Indices

Negative indices count from the end of the list.

```python
numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]

print(numbers[-3:])
# Prints [7, 8, 9]
