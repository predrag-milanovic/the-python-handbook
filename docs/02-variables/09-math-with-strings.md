# Math With Strings

When working with strings, the `+` operator performs [concatenation](https://en.wikipedia.org/wiki/Concatenation), which means joining two strings together.

In general, it is better to use string interpolation with f-strings than `+` concatenation. F-strings are easier to read when you are combining text with variable values.

```python
first_name = "Predrag "
last_name = "Milanovic"
full_name = first_name + last_name

print(full_name)
# Predrag Milanovic
```

The `full_name` variable now holds the value `"Predrag Milanovic"`.

Notice the extra space at the end of `"Lane "` in the `first_name` variable. That space is there so the two words are separated correctly in the final result.
