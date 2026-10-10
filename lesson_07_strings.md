# Lesson 7: Strings

## What is a string?
A string is text inside quotation marks.

## Indexing
Each character has a position number called an index. Counting starts at 0.

    word = "Python"
    print(word[0])    # P
    print(word[-1])   # n (negative indexes count from the end)

## Slicing
A slice takes a piece of a string: `text[start:end]`. The end position is not included.

    print(word[0:2])  # Py

## Useful methods
- `.upper()` and `.lower()` change case.
- `.strip()` removes spaces at the ends.
- `.replace(old, new)` swaps text.
- `len()` counts characters.

## Formatting
An f-string puts values inside text. Put an `f` before the quotes and wrap variables in braces.

    name = "Ada"
    print(f"Hello, {name}!")

## Practice exercises
1. Print the length of your name using `len()`.
2. Print your name in capital letters.
3. Use an f-string to print a sentence with your age.

## Common beginner mistakes
- Starting to count from 1 instead of 0.
- Trying to change a character in place. Strings cannot be changed; make a new one.
- Forgetting the `f` before an f-string.

## Recap
- Strings are text, indexed from 0.
- Use methods and f-strings to work with them.

## Challenge
Ask the user for a word and print it backwards.

## Example code

```python
# Lesson 7 example: strings

word = "Python"

print("First letter:", word[0])
print("Last letter:", word[-1])
print("First two letters:", word[0:2])
print("Length:", len(word))

# Change case and clean spaces
greeting = "   hello there   "
print(greeting.strip().upper())

# f-string for formatting
name = "Ada"
age = 10
print(f"{name} is {age} years old.")
```
