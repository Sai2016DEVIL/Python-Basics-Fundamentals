# Lesson 8: If, Elif and Else

## Making decisions
An `if` statement runs code only when a condition is `True`.

    temperature = 25
    if temperature > 20:
        print("It is warm.")

## Indentation matters
The indented lines belong to the `if`. Use four spaces for each level.

## elif and else
    score = 72
    if score >= 90:
        print("Grade A")
    elif score >= 70:
        print("Grade B")
    else:
        print("Keep practising")

## Practice exercises
1. Print "adult" if an age is 18 or more, otherwise print "minor".
2. Print whether a number is zero, positive, or negative.
3. Check whether a password equals a fixed word and print the result.

## Common beginner mistakes
- Forgetting the colon at the end of the `if` line.
- Wrong indentation, which causes an IndentationError.
- Using `=` instead of `==` in the condition.

## Recap
- `if` checks a condition.
- `elif` adds more checks; `else` handles everything left.

## Challenge
Ask for a number and say whether it is even or odd.

## Example code

```python
# Lesson 8 example: if, elif and else

score = 72

if score >= 90:
    print("Grade A")
elif score >= 70:
    print("Grade B")
else:
    print("Keep practising")

# A simple yes or no check
password = "sunshine"
if password == "sunshine":
    print("Access granted")
else:
    print("Access denied")
```
