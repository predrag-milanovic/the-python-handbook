# Bitwise "&" Operator

Bitwise operators are similar to logical operators, but they work on the bits inside numbers instead of on boolean values.

With bitwise AND, Python compares each bit in the same position and keeps a `1` only when both bits are `1`.

```python
0 & 0 = 0
1 & 1 = 1
1 & 0 = 0
```

For example, `5` and `7` in binary are:

- `0101` is `5`
- `0111` is `7`

```python
0101
&
0111
=
0101
```

So `5 & 7` is `5`.

Another example:

- `0101` is `5`
- `0010` is `2`

```python
0101
&
0010
=
0000
```

So `5 & 2` is `0`.

## Binary Notation

When writing a number in [binary](https://en.wikipedia.org/wiki/Binary_code), the `0b` prefix tells Python that the value is binary. For example, `0b10` is two in binary, while `10` without the prefix is just ten.

## In Python

The ampersand `&` is the bitwise AND operator in Python.

```python
print(0b0101 & 0b0111)
# Prints 5

binary_five = 0b0101
binary_seven = 0b0111
print(binary_five & binary_seven)
# Prints 5
```

Leading zeros are often added for clarity, but they do not change the value of a binary number.

## Guild Permissions

Bitwise operators are useful for storing multiple yes/no flags in a single number. A common example is user permissions.

Imagine a game called Fantasy Quest where a user can have four guild permissions:

- `can_create_guild` - leftmost bit (`0b1000`)
- `can_review_guild` - second bit from the left (`0b0100`)
- `can_delete_guild` - second bit from the right (`0b0010`)
- `can_edit_guild` - rightmost bit (`0b0001`)

If a user has no permissions, their binary value is `0b0000`.

If a user only has `can_create_guild`, their binary value is `0b1000`. If they have `can_review_guild` and `can_edit_guild`, their value is `0b0101`.

To check whether a user has a specific permission, compare their permissions with the bit for that permission using `&`.

```python
user_permissions = 0b0101
can_review_guild = 0b0100

# Perform bitwise AND to get the user's review permission.
user_review_guild_permission = user_permissions & can_review_guild

# If the result is 0b0100, the user has the review permission.
```
