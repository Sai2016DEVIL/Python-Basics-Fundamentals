# Lesson 17: Booleans and Logic

## Boolean values
A boolean is `True` or `False`. Comparisons produce booleans.

    print(5 > 3)    # True

## Logical operators
- `and`: `True` only if both sides are `True`.
- `or`: `True` if at least one side is `True`.
- `not`: flips the value.

    age = 15
    has_ticket = True
    print(age >= 12 and has_ticket)   # True

## Truthy and falsy
Empty values such as `""`, `0`, and `[]` count as `False` in a condition.

## Practice exercises
1. Check whether a number is between 1 and 10 using `and`.
2. Print whether it is raining or it is sunny using `or`.
3. Use `not` to flip a boolean variable and print it.

## Common beginner mistakes
- Writing `if x == 1 or 2` instead of `if x == 1 or x == 2`.
- Confusing `and` with `or`.

## Recap
- Booleans are `True` or `False`.
- Combine conditions with `and`, `or`, and `not`.

## Challenge
Write a program that decides whether a user can watch a film, based on their age and whether they have a parent with them.

## Example code

```python
# Lesson 17 example: booleans and logic

age = 15
has_ticket = True

print("Can enter?", age >= 12 and has_ticket)

# or: at least one must be True
is_weekend = False
is_holiday = True
print("Day off?", is_weekend or is_holiday)

# not flips True and False
print("Not weekend:", not is_weekend)

# Check a range
number = 7
if 1 <= number <= 10:
    print("Number is between 1 and 10")
```
