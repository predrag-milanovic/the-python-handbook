# Functions

Functions allow us to reuse and organize code.

For example, say we want to calculate the area of a circle:

```python
radius = 5
area = 3.14 * radius * radius
```

That works. But what if we want to calculate the area of other circles, each with a different radius?

We could copy the code and change the variable names:

```python
radius = 5
area1 = 3.14 * radius * radius

radius2 = 7
area2 = 3.14 * radius2 * radius2
```

This works too, but it repeats the same logic over and over again. If we want to calculate the area of many circles, repeating the code becomes wasteful and harder to maintain.

Instead, we can define a function called `area_of_circle` using the `def` keyword:

```python
def area_of_circle(r):
	pi = 3.14
	result = pi * r * r
	return result
```

Let's break this function down:

The function takes one input called `r`. This input is called a parameter.
The indented lines after the `:` make up the function body. This is the code that runs when the function is called.
The function returns a single value. In this case, it returns the value stored in `result`.

To [call](https://en.wikibooks.org/wiki/Python_Programming/Functions#Function_Calls) the function, pass in a value for `r` and store the result in a variable:

```python
area = area_of_circle(5)
print(area)
# 78.5
```

Here is what happens:

`5` is passed into the function as the argument for `r`.
The function body runs and stores `78.5` in `result`.
The `return` statement sends `result` back out of the function.
The `area_of_circle(5)` expression evaluates to `78.5`, so `area` stores that value.

Because the function is already defined, we can use it again and again with different inputs:

```python
area = area_of_circle(6)
print(area)
# 113.04

area = area_of_circle(7)
print(area)
# 153.86
```

Functions make our code easier to reuse, easier to read, and easier to change.
