# Lesson 15: Handling Errors

## Errors happen
When Python meets a problem it cannot handle, it raises an exception and stops. You can catch the exception and respond gracefully.

## try and except
    try:
        number = int(input("Enter a number: "))
        print("Double:", number * 2)
    except ValueError:
        print("That was not a whole number.")

## else and finally
- `else` runs when no error happened.
- `finally` runs whether or not there was an error.

## Common exceptions
- `ValueError`: right type, wrong value, e.g. `int("hello")`.
- `TypeError`: wrong type, e.g. `"5" + 5`.
- `ZeroDivisionError`: dividing by zero.
- `IndexError`: list position does not exist.
- `KeyError`: dictionary key does not exist.

## Practice exercises
1. Catch a `ZeroDivisionError` when dividing by a user-entered number.
2. Use `try` and `except` to handle a bad list index.
3. Add an `else` block that prints "Success" when no error happens.

## Common beginner mistakes
- Using a bare `except:` for everything, which hides real bugs. Name the exception.
- Putting too much code inside `try`. Keep it small.

## Recap
- `try` holds risky code; `except` handles errors.
- Name the exception you expect.

## Challenge
Ask for two numbers and divide them. Handle both invalid input and division by zero.

## Example code

```python
# Lesson 15 example: handling errors

# Safely convert user input to a number
try:
    number = int(input("Enter a whole number: "))
    print("Double:", number * 2)
except ValueError:
    print("That was not a whole number.")
else:
    print("Conversion worked.")
finally:
    print("Thanks for trying.")

# Catch a list index error
items = ["a", "b"]
try:
    print(items[5])
except IndexError:
    print("That position does not exist.")
```
