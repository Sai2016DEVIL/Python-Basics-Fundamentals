# Lesson 12: Dictionaries

## What is a dictionary?
A dictionary stores pairs of a key and a value, written with curly brackets. You look up a value using its key.

    pet = {"name": "Biscuit", "age": 3}
    print(pet["name"])      # Biscuit

## Adding and changing
    pet["colour"] = "brown"   # add a new key
    pet["age"] = 4            # change an existing value

## Safe lookups
If a key does not exist, `pet["weight"]` causes a KeyError. Use `.get()` instead:

    print(pet.get("weight", "unknown"))   # prints "unknown"

## Looping
    for key, value in pet.items():
        print(key, "=", value)

## Practice exercises
1. Create a dictionary about a book with title, author, and pages.
2. Print one value from the dictionary.
3. Add a new key and print the whole dictionary.

## Common beginner mistakes
- Using square brackets when you need curly brackets to create the dictionary.
- Looking up a key that does not exist without using `.get()`.

## Recap
- Dictionaries map keys to values.
- Use `.get()` for safe lookups.

## Challenge
Store a list of three friends' names and favourite colours in dictionaries, then print each friend's colour.

## Example code

```python
# Lesson 12 example: dictionaries

pet = {"name": "Biscuit", "age": 3}

print("Pet name:", pet["name"])

# Add and change values
pet["colour"] = "brown"
pet["age"] = 4
print(pet)

# Safe lookup with a default value
print("Weight:", pet.get("weight", "unknown"))

# Loop through keys and values
for key, value in pet.items():
    print(key, "=", value)
```
