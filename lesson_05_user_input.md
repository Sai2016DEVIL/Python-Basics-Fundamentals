# Lesson 5: User Input

## input()
`input()` pauses the program and waits for the user to type something. It always returns text.

    name = input("What is your name? ")
    print("Hello,", name)

## Converting input
Because `input()` returns a string, convert it when you need a number.

    age = int(input("How old are you? "))
    print("Next year you will be", age + 1)

## Validating input
Users make mistakes. You can check the value before using it. Use `try` with `int()` and a loop to ask again.

## Practice exercises
1. Ask for the user's favourite food and print a sentence about it.
2. Ask for two numbers and print their sum.
3. Ask for a number and print whether it is positive or not.

## Common beginner mistakes
- Forgetting that `input()` returns text, so `"5" + 5` fails.
- Entering letters when the program expects a number, which causes a ValueError.

## Recap
- `input()` gets text from the user.
- Convert with `int()` or `float()` for numbers.
- Validate before you trust the value.

## Challenge
Ask the user for their birth year and print their approximate age this year.

## Example code

```python
# Lesson 5 example: user input

# Ask for a name
name = input("What is your name? ")
print("Nice to meet you,", name)

# Ask for an age and convert it to a whole number
age_text = input("How old are you? ")

# Check that the input contains only digits before converting
if age_text.isdigit():
    age = int(age_text)
    print("In five years you will be", age + 5)
else:
    print("Please type a whole number next time.")
```
