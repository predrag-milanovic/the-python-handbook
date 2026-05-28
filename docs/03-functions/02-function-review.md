# Function Review

Functions can feel tricky at first, and that is normal. It takes a little time to get used to them, but once they click, they become second nature.

Let's break this function down line by line:

```python
def area_of_circle(r):
	pi = 3.14
	result = pi * r * r
	return result

radius = 5
area = area_of_circle(radius)
print(area)
# 78.5
```

Here is what happens, in order:

`def area_of_circle(r):`
The function is defined for later use. It is not called yet, so the body is ignored for now.

`radius = 5`
A new variable called `radius` is created and set to `5`.

`area = area_of_circle(radius)`
The function is called with `radius` as the input. Since `radius` holds `5`, that value is passed into the function.

`def area_of_circle(r):`
Execution jumps into the function body, and `r` is set to `5`.

`pi = 3.14`
A new variable called `pi` is created with the value `3.14`.

`result = pi * r * r`
Python calculates `3.14 * 5 * 5` and stores the answer in `result`.

`return result`
The function sends `result` back as output.

`area = area_of_circle(radius)`
The returned value, `78.5`, is stored in the `area` variable.

`print(area)`
The value of `area` is printed to the console.

When you read code like this, it helps to follow the flow from top to bottom and remember that a function body only runs when the function is called.
