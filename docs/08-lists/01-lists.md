# Lists

A natural way to organize and store data is in a list. Some languages call them "arrays," but in Python we call them lists.

Think about the apps you use every day and how often data appears in list form:

- An X (formerly Twitter) feed is a list of posts.
- An online store is a list of products.
- The state of a chess game can be represented as a list of moves.
- This bullet list is a list of things that are lists.

## Creating a List

In Python, lists are created with square brackets `[]`, and each item is separated by a comma:

```python
inventory = ["Iron Breastplate", "Healing Potion", "Leather Scraps"]
```

This is a list of strings.

## List Items and Data Types

Lists can store items of any data type, including numbers, strings, booleans, and even other lists.

For now, focus on this key idea: a list is one variable that can hold many values in order.

## Multi-line List Formatting

When you create lists manually, putting every item on one line can become hard to read.

You can split a list across multiple lines:

```python
flower_types = [
	"daffodil",
	"rose",
	"chrysanthemum"
]

player_ages = [
	23,
	18,
	31,
	42
]
```

This style improves readability and organization, especially when lists have many items or long values.

It is still the same Python list syntax. In other words, this is a formatting choice, not a behavior change.
