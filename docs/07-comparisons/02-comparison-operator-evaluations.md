# Comparison Operator Evaluations

When you use a comparison operator, the result is always a boolean value: `True` or `False`.

For example, these two lines do the same thing:

```python
is_bigger = 5 > 4
```

```python
is_bigger = True
```

In both cases, `is_bigger` ends up holding the boolean value `True`.

Why? Because `5` is greater than `4`, so the comparison `5 > 4` evaluates to `True`.

Comparison Practice

```python
car_size = 4
truck_size = 5
is_smaller = car_size < truck_size
```

Here, `is_smaller` is assigned `True` because `car_size` is less than `truck_size`.
