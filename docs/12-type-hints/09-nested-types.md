# Nested Types

We've looked at relatively simple container types such as `list[str]`, but containers can also hold other containers. These are called **nested container types**.

For example, a dictionary could map each character's name to their list of spells:

```python
character_spells: dict[str, list[str]] = {
	"Gandalf": ["Fireball", "Light"],
	"Frodo": ["Hide"],
}
```

Read `dict[str, list[str]]` from the outside in:

- it is a dictionary (`dict`)
- each key is a string (`str`)
- each value is a list of strings (`list[str]`)

Nested types can become confusing when they describe several layers of containers. Even so, the type hint is often clearer than having no type information at all. For now, remember that type hints can describe containers within containers.
