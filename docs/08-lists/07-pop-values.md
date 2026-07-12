# Pop Values

`.pop()` is the opposite of `.append()`. While `.append()` adds a value to the end of a list, `.pop()` removes the last value and returns it so you can use it again.

```python
vegetables = ["broccoli", "cabbage", "kale", "tomato"]
last_vegetable = vegetables.pop()

print(vegetables)
# ['broccoli', 'cabbage', 'kale']

print(last_vegetable)
# 'tomato'
```
