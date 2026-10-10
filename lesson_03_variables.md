# Lesson 3: Variables

## What is a variable?
A variable is a named box that stores a value. You create one with the `=` sign, which is called assignment.

    score = 10
    name = "Ada"

`score` now holds the value 10.

## Naming rules
- Use letters, numbers, and underscores (`_`).
- Start with a letter or underscore, not a number.
- No spaces. Use `high_score`, not `high score`.
- Avoid Python keywords such as `if`, `for`, and `print`.

Good names describe what the value means: `player_age` is better than `x`.

## Changing a variable
You can give a variable a new value at any time.

    score = 10
    score = 25
    print(score)   # prints 25

## Using variables in calculations
    apples = 4
    pears = 3
    total = apples + pears
    print(total)   # prints 7

## Practice exercises
1. Create a variable `city` with your city name and print it.
2. Create two number variables, add them, and print the result.
3. Change a variable's value and print it before and after the change.

## Common beginner mistakes
- Using a name that was never assigned, which causes a NameError.
- Writing `score == 10` when you mean `score = 10`. Double equals compares; single equals assigns.
- Starting a name with a number, such as `1st_place`.

## Recap
- `=` stores a value in a variable.
- Pick clear, lowercase names with underscores.

## Challenge
Create variables for a book's title, page count, and pages read. Print how many pages are left.

## Example code

```python
# Lesson 3 example: variables

# Store values in variables
player_name = "Ada"
player_score = 10

# Print them
print(player_name, "has a score of", player_score)

# Change the score
player_score = player_score + 15
print("New score:", player_score)

# Use variables in a calculation
bonus = 5
final_score = player_score + bonus
print("Final score:", final_score)
```
