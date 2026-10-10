# Lesson 10: For Loops

## for loops and range()
A `for` loop repeats code for each item in a sequence. `range()` creates a sequence of numbers.

    for i in range(3):
        print(i)     # prints 0, 1, 2

`range(start, stop)` stops before `stop`:

    for i in range(1, 6):
        print(i)     # prints 1 to 5

`range(start, stop, step)` changes the step size:

    for i in range(0, 11, 2):
        print(i)     # 0, 2, 4, 6, 8, 10

## Looping over text
    for letter in "Py":
        print(letter)

## Practice exercises
1. Print the numbers 1 to 10.
2. Print only the even numbers from 2 to 20.
3. Loop over the letters of your name and print each one on its own line.

## Common beginner mistakes
- Expecting `range(5)` to include 5. It stops at 4.
- Forgetting the colon after `for`.

## Recap
- `for` loops visit each item.
- `range()` produces numbers for counting.

## Challenge
Print a multiplication table for 7 from 1 to 10.

## Example code

```python
# Lesson 10 example: for loops

# Count from 0 to 4
for i in range(5):
    print("Number:", i)

# Count by twos
for n in range(2, 11, 2):
    print("Even:", n)

# Loop over each letter of a word
for letter in "Ada":
    print("Letter:", letter)
```
