# Printing vs. Returning

Some new developers get hung up on the difference between `print()` and `return`. When exercises or test harnesses print your function output to the console, it can make `print()` and `return` look interchangeable — but they are not.

What `print()` does
- Sends text to the console (a side effect).
- Always returns `None` — it does not provide a usable value to the caller.

What `return` does
- Ends a function's execution and sends a value back to the caller.
- Does not print anything by itself; the caller decides if and when to print the returned value.

Example

```python
def say_with_print():
	print("hello")

def say_with_return():
	return "hello"

x = say_with_print()   # prints "hello"; x is None
y = say_with_return()  # nothing printed; y == "hello"
print(y)                # now "hello" is printed
```

Why printed tests are confusing

Some learning platforms show function results by printing them. That helps you see output when running scripts, but it can hide the difference between producing a value (`return`) and merely displaying it (`print`). Automated tests may either inspect returned values or capture console output — write your functions to return values when callers should use the result.

Using `print()` to debug

Adding `print()` statements while developing is a quick way to inspect values and program flow. It's a helpful habit for debugging, but remember to remove or replace debugging prints before finalizing code. Leftover `print()` calls can interfere with automated tests that expect specific return values or controlled console output.
