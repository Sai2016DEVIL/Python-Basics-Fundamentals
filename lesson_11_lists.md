# Lesson 11: Lists

## What is a list?
A list stores several values in one variable, in order, inside square brackets.

    fruits = ["apple", "banana", "cherry"]

## Indexes
List positions start at 0, just like strings.

    print(fruits[0])    # apple
    print(fruits[-1])   # cherry

## Changing a list
    fruits.append("date")       # add to the end
    fruits[1] = "blueberry"     # replace an item
    fruits.remove("apple")      # remove an item by value
    print(len(fruits))          # count the items

## Looping through a list
    for fruit in fruits:
        print(fruit)

## Practice exercises
1. Create a list of three of your favourite foods and print the first one.
2. Add a new item to the list and print the list length.
3. Loop through a list of numbers and print each number doubled.

## Common beginner mistakes
- Using an index that is too large, which causes an IndexError.
- Forgetting that `append()` changes the list in place and returns nothing. Do not write `x = x.append(...)`.

## Recap
- Lists hold ordered items.
- Use indexes, `append()`, and loops to work with them.

## Challenge
Keep a list of scores entered by the user and print the highest one.

## Example code

```python
# Lesson 11 example: lists

fruits = ["apple", "banana", "cherry"]

print("First fruit:", fruits[0])
print("Last fruit:", fruits[-1])

# Add and change items
fruits.append("date")
fruits[1] = "blueberry"
print("Updated list:", fruits)

# Loop through the list
for fruit in fruits:
    print("I like", fruit)

# Doubling numbers
numbers = [1, 2, 3]
for n in numbers:
    print(n * 2)
```
