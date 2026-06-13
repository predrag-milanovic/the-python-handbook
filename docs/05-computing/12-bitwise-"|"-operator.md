# Bitwise "|" Operator

Bitwise operators work on the bits inside numbers instead of on boolean values.

The bitwise OR operator keeps a `1` in any position where either bit is `1`.

```text
0 | 0 = 0
1 | 1 = 1
1 | 0 = 1
```

For example, `5` and `7` in binary are:

- `0101` is `5`
- `0111` is `7`

```text
0101
|
0111
=
0111
```

So `5 | 7` is `7`.

Another example:

- `0101` is `5`
- `0010` is `2`

```text
0101
|
0010
=
0111
```

So `5 | 2` is also `7`.

## Binary Notation

When writing a number in [binary](https://en.wikipedia.org/wiki/Binary_code), the `0b` prefix tells Python that the value is binary. For example, `0b10` is two in binary, while `10` without the prefix is just ten.

## In Python

The pipe symbol `|` is the bitwise OR operator in Python.

```python
print(0b0101 | 0b0111)
# Prints 7

binary_five = 0b0101
binary_seven = 0b0111
print(binary_five | binary_seven)
# Prints 7
```

Leading zeros are often added for clarity, but they do not change the value of a binary number.

## Guild Permissions

Bitwise OR is useful when you want to combine permissions or flags.

Imagine a game called Fantasy Quest where a guild has four permissions:

- `can_invite` - leftmost bit (`0b1000`)
- `can_kick` - second bit from the left (`0b0100`)
- `can_enter_dungeon` - second bit from the right (`0b0010`)
- `can_surrender` - rightmost bit (`0b0001`)

If players are in a guild together, they gain all the permissions of the other members of the guild.

For example, if Jack has `can_invite` and Jill has `can_kick`, their combined permissions should include both bits:

```text
Jack: 0b1000
Jill: 0b0100
      -------
Both: 0b1100
```

In Python, you can combine the permissions with `|`:

```python
jack_permissions = 0b1000
jill_permissions = 0b0100

guild_permissions = jack_permissions | jill_permissions
# guild_permissions is 0b1100
```
