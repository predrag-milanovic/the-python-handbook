# Floor Division

Python has strong built-in support for mathematical operations. This is one of the reasons it is so widely used in artificial intelligence, machine learning, and data science.

Floor division works like normal division, except the result is floored afterward. That means it is rounded down to the nearest integer. Use the `//` operator when you want floor division.

```python
7 // 3
# 2 (an integer, rounded down from 2.333)

-7 // 3
# -3 (an integer, rounded down from -2.333)
```

Note that floor division rounds toward negative infinity, not toward zero. That is why `-7 // 3` becomes `-3` instead of `-2`.
