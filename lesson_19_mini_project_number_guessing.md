# Lesson 19: Mini Project - Number Guessing Game

## The goal
Build a game where the computer picks a secret number and the player guesses it. The game says "too high" or "too low" until the player wins.

## Ideas used
- `random` to pick the secret number.
- `while` loop to keep the game going.
- `input()` with validation.
- `if`, `elif`, and `else` to compare guesses.
- `try` and `except` for bad input.

## Step by step
1. Import `random`.
2. Pick a number from 1 to 100 with `random.randint(1, 100)`.
3. Loop until the guess is correct.
4. Convert and validate input.
5. Compare the guess and give a hint.
6. Count the attempts.

## Practice exercises
1. Change the range to 1 to 50.
2. Print a message when the player uses fewer than five guesses.
3. Add a message for guesses outside the range.

## Common beginner mistakes
- Forgetting to convert input to an integer before comparing.
- Creating the secret number inside the loop, so it changes every time.

## Recap
- Combine loops, conditions, input, and random numbers to build a complete program.

## Challenge
Let the player choose the range before the game starts.

## Example code

```python
# Lesson 19 example: number guessing game

import random

secret = random.randint(1, 100)   # computer picks a secret number
attempts = 0
print("I am thinking of a number between 1 and 100.")

while True:
    guess_text = input("Your guess: ")

    # Validate the input before using it
    if not guess_text.isdigit():
        print("Please type a whole number.")
        continue

    guess = int(guess_text)
    attempts = attempts + 1

    if guess < 1 or guess > 100:
        print("Stay between 1 and 100.")
    elif guess < secret:
        print("Too low!")
    elif guess > secret:
        print("Too high!")
    else:
        print("Correct! You needed", attempts, "attempts.")
        break
```
