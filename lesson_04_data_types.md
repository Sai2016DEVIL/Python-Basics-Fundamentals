# Lesson 4: Data Types

## Main types
- **str** (string): text, such as `"hello"`.
- **int** (integer): whole numbers, such as `7`.
- **float**: numbers with a decimal point, such as `3.14`.
- **bool** (boolean): `True` or `False`.

## Checking a type
`type()` tells you what kind of value you have.

    print(type(7))        # <class 'int'>
    print(type("7"))      # <class 'str'>

Notice that `7` and `"7"` look similar but are different types.

## Type conversion
You can change one type to another.

    age_text = "10"
    age = int(age_text)     # text becomes a whole number
    price = float("2.50")   # text becomes a decimal number
    label = str(42)         # number becomes text

## Practice exercises
1. Use `type()` on five different values and note each result.
2. Convert the text `"25"` to an integer and add 5 to it.
3. Convert the number `9.99` to text and print it.

## Common beginner mistakes
- Trying to add text and a number directly: `"5" + 3` causes a TypeError. Convert first.
- Using `int()` on text with a decimal, such as `int("2.5")`, which causes a ValueError.

## Recap
- Python has str, int, float, and bool.
- `type()` identifies a value's type.
- `int()`, `float()`, and `str()` convert between types.

## Challenge
Write a program that stores a price as text, converts it to a float, adds tax of 20 percent, and prints the total.

## Example code

```python
# Lesson 4 example: data types

# Different types
name = "Ada"          # str
age = 10              # int
height = 1.42         # float
is_student = True     # bool

print(name, type(name))
print(age, type(age))
print(height, type(height))
print(is_student, type(is_student))

# Convert text to a number and do maths
age_text = "10"
next_year_age = int(age_text) + 1
print("Next year:", next_year_age)

# Convert a number to text
score = 95
message = "Score: " + str(score)
print(message)
```
