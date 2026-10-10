# Lesson 9: While Loops

## What is a loop?
A loop repeats code. A `while` loop keeps repeating as long as its condition is `True`.

    count = 1
    while count <= 3:
        print(count)
        count = count + 1

## Avoiding endless loops
Always change something inside the loop so the condition eventually becomes `False`. Otherwise the loop never stops.

## break
`break` leaves the loop immediately.

## Practice exercises
1. Print the numbers 1 to 5 with a `while` loop.
2. Count down from 10 to 1, then print "Liftoff!".
3. Keep asking for a word until the user types "stop".

## Common beginner mistakes
- Forgetting to update the counter, which causes an endless loop. Press Ctrl+C to stop it.
- Off-by-one errors: using `<` when you meant `<=`.

## Recap
- `while` repeats while a condition is `True`.
- Update your variables so the loop ends.

## Challenge
Keep asking the user to guess a secret number until they get it right, then print how many tries it took.

## Example code

```python
# Lesson 9 example: while loops

# Count from 1 to 3
count = 1
while count <= 3:
    print("Count:", count)
    count = count + 1  # increase the counter so the loop ends

print("Loop finished.")

# Stop early with break
total = 0
while True:
    number = 5
    total = total + number
    if total >= 15:
        break
print("Total reached:", total)
```
