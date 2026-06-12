
# Logical operators

Logical operators work with boolean values: `True` and `False`.

- `and`: returns `True` only if both operands are `True`.
- `or`: returns `True` if at least one operand is `True`.

Truth-table examples:

```python
True and True   == True
True and False  == False
False and False == False

True or True    == True
True or False   == True
False or False  == False
```

Python examples:

```python
print(True and True)
# prints True

print(True or False)
# prints True
```

Nesting and evaluation

You can nest logical expressions using parentheses to make the intended order explicit.

```python
print((True or False) and False)
# prints False
```

Step-by-step evaluation of the nested example:

1. Evaluate the parenthesized expression: `(True or False)` → `True`.
2. Then evaluate `True and False` → `False`.

Operator precedence notes

By default, `and` has higher precedence than `or`. Use parentheses to ensure the order you want.
