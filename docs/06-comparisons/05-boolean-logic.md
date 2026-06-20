# Boolean Logic

Boolean logic refers to logic dealing with boolean (`True` or `False`) values. For example:

- Dogs must have four legs *and* weigh less than 100 kilograms. (Both conditions must be true)
- Cars are cool if they go faster than 200 MPH, *or* if they are electric. (At least one condition must be true)

## Logical Operators Review

As we discussed earlier, the logical operators `and` and `or` can be used to perform boolean logic.

### And Review

The `and` operator returns `True` if *both* of the conditions on either side evaluates to `True`:

```python
def is_dog(num_legs, weight):
    return num_legs == 4 and weight < 100
```

Let's go over how this function evaluates the parameters `num_legs=4` and `weight=99`:

```python
return 4 == 4 and 99 < 100
```

```python
return True and True
```

```python
return True
```

Let's see what would happen with `num_legs=3` and `weight=98` instead:

```python
return 3 == 4 and 98 < 100
```

```python
return False and True
```

```python
return False
```

### Or Review

The `or` operator returns `True` if *at least one* of the conditions on either side evaluates to `True`:

```python
def is_car_cool(speed, is_electric):
    return speed > 200 or is_electric
```

Let's use a non-electric car that can do 250 MPH:

```python
return 250 > 200 or False
```

```python
return True or False
```

```python
return True
```
