# Lesson 13: Functions

## What is a function?
A function is a named block of code you can reuse. Define it with `def`.

    def greet(name):
        print("Hello,", name)

    greet("Ada")

## Parameters and arguments
The name in brackets (`name`) is a parameter. The value you pass in (`"Ada"`) is an argument.

## return
`return` sends a value back to the caller.

    def add(a, b):
        return a + b

    total = add(3, 4)   # total is 7

## Scope
A variable created inside a function exists only inside it. This is called local scope.

## Practice exercises
1. Write a function that prints your name.
2. Write a function that takes two numbers and returns their product.
3. Write a function that returns "even" or "odd" for a number.

## Common beginner mistakes
- Forgetting `return` and then printing `None`.
- Forgetting the colon after `def`.
- Trying to use a local variable outside the function.

## Recap
- `def` creates a function.
- Parameters receive inputs; `return` gives back a result.

## Challenge
Write a function that takes a temperature in Celsius and returns it in Fahrenheit.

## Example code

```python
# Lesson 13 example: functions

def greet(name):
    # Print a greeting for the given name
    print("Hello,", name)

def add(a, b):
    # Return the sum of two numbers
    return a + b

def is_even(number):
    # Return True if the number is even
    return number % 2 == 0

greet("Ada")
result = add(3, 4)
print("3 + 4 =", result)
print("Is 10 even?", is_even(10))
```
