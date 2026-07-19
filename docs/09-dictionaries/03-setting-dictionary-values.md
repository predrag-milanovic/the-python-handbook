# Setting Dictionary Values

You do not need to create a dictionary with all of its values already inside. A common pattern is to start with a blank dictionary and add keys later as new values become available.

Setting a value uses the same square-bracket syntax as reading a value, but with the assignment operator (`=`).

```python
planets = {}
planets["Earth"] = True
planets["Pluto"] = False

print(planets["Pluto"])
# Prints: False
```
