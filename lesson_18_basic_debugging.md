# Lesson 18: Basic Debugging

## What is debugging?
Debugging means finding and fixing mistakes in code. Every programmer does it daily.

## Read the error message
A traceback shows the file, the line number, and the error type. Start with the last line, then check the line it names.

## Common error types
- **SyntaxError**: the code is not valid Python, such as a missing colon or quote.
- **IndentationError**: lines are indented incorrectly.
- **NameError**: a variable is used before it exists or is misspelled.
- **TypeError**: an operation uses the wrong type, e.g. `"5" + 5`.
- **ValueError**: the type is right but the value is not, e.g. `int("abc")`.

## Debugging strategies
1. Read the error message carefully.
2. Print variables to see their actual values.
3. Change one thing at a time.
4. Explain the code line by line, out loud.

## Practice exercises
1. Find the missing colon in `if x > 3` and fix it.
2. Fix a NameError caused by a misspelled variable.
3. Fix a TypeError by converting a string to an integer.

## Common beginner mistakes
- Changing many lines at once, so you do not know what fixed it.
- Ignoring the line number in the error message.

## Recap
- Read the error, then the line it names.
- Print values to find what is really happening.

## Challenge
Here is broken code: `total = "5" + 10`. Fix it so the total is 15.

## Example code

```python
# Lesson 18 example: basic debugging

# Each block below shows a common error and its fix.

# 1. TypeError: fixed by converting text to a number
text_number = "5"
total = int(text_number) + 10
print("Total:", total)

# 2. NameError: fixed by spelling the name correctly
player_score = 20
print("Score:", player_score)

# 3. Printing values to inspect them while debugging
values = [3, 7, 2]
for v in values:
    print("Debug value:", v)
```
