# Lesson 14: Imports and Modules

## What is a module?
A module is a file of ready-made code. Python includes many in its standard library.

## import
    import random
    print(random.randint(1, 6))   # random number from 1 to 6

You can also import one function:

    from math import sqrt
    print(sqrt(16))   # 4.0

## Useful standard modules
- `random`: random choices and numbers.
- `math`: square roots, pi, and more.
- `datetime`: dates and times.

## Practice exercises
1. Import `math` and print the value of `math.pi`.
2. Use `random.choice()` on a list of colours and print one.
3. Print today's date using `datetime.date.today()`.

## Common beginner mistakes
- Naming your own file `random.py`, which hides the real module.
- Forgetting the module name before a function, such as writing `randint` without `random.`.

## Recap
- `import` brings in code from other modules.
- Use `module.function()` or `from module import function`.

## Challenge
Write a program that picks a random number between 1 and 100 and prints whether it is above or below 50.

## Example code

```python
# Lesson 14 example: imports and modules

import random
import math
from datetime import date

# Random number between 1 and 6, like a dice
print("Dice roll:", random.randint(1, 6))

# Pick a random item from a list
colours = ["red", "blue", "green"]
print("Random colour:", random.choice(colours))

# Use the math module
print("Pi is about", round(math.pi, 2))

# Today's date
print("Today is", date.today())
```
