# List Updates

You can change an existing item in a list by assigning a new value to its index. This updates the item in place instead of creating a new list.

For example, we can change `Leather` to `Leather Armor` in the `inventory` list:

```python
inventory = ["Leather", "Iron Ore", "Healing Potion"]
inventory[0] = "Leather Armor"

print(inventory)
# ['Leather Armor', 'Iron Ore', 'Healing Potion']
```
