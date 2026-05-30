# Order of Functions

All functions must be defined before they're used at runtime.

That may sound like it makes ordering your code difficult, but there's a simple convention that solves the problem: define your helper functions first, then call a single entry-point function at the end of the file. That ensures every `def` has been executed by the Python interpreter before the program starts doing work.

By convention the entry-point is often named `main`:

```python
def main():
	health = 10
	armor = 5
	add_armor(health, armor)

def add_armor(h, a):
	new_health = h + a
	print_health(new_health)

def print_health(new_health):
	print(f"The player now has {new_health} health")

# Call the entry point at the end of the file
main()
```

A small but common improvement is to protect the entry point so the file can be imported as a module without running the script immediately:

```python
if __name__ == "__main__":
	main()
```

That pattern runs `main()` only when the file is executed directly, not when its functions are imported elsewhere.

In short: organize code by defining functions first, then call a clear entry point. This keeps ordering predictable and makes your code easier to reuse and test.

