# Lesson 6: Math and Operators

## Arithmetic operators
- `+` addition
- `-` subtraction
- `*` multiplication
- `/` division (always gives a float)
- `//` integer division (rounds down)
- `%` remainder (modulus)
- `**` power

    print(7 + 3)    # 10
    print(7 / 2)    # 3.5
    print(7 // 2)   # 3
    print(7 % 2)    # 1
    print(2 ** 3)   # 8

## Comparison operators
These return `True` or `False`: `==`, `!=`, `<`, `>`, `<=`, `>=`.

## Order of operations
Python follows the usual maths order: brackets, powers, multiplication and division, then addition and subtraction. Use brackets to make your intention clear.

## Practice exercises
1. Calculate the area of a rectangle that is 6 wide and 4 tall.
2. Find the remainder when 17 is divided by 5.
3. Check whether 10 is greater than 7 and print the result.

## Common beginner mistakes
- Using `=` instead of `==` when comparing.
- Expecting `/` to round. It keeps decimals; use `//` for whole results.
- Forgetting that `%` gives the remainder, not a percentage.

## Recap
- Operators combine and compare values.
- `%` gives the remainder.

## Challenge
Ask the user for a number of seconds and print how many whole minutes and leftover seconds that makes.

## Example code

```python
# Lesson 6 example: math and operators

a = 17
b = 5

print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
print("Whole division:", a // b)
print("Remainder:", a % b)
print("Power:", 2 ** 4)

# Comparisons give True or False
print("Is a bigger than b?", a > b)
print("Are they equal?", a == b)
```
