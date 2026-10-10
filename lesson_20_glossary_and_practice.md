# Lesson 20: Glossary and Practice

## Glossary
- **Argument**: a value passed into a function.
- **Boolean**: a `True` or `False` value.
- **Comment**: text after `#` that Python ignores.
- **Dictionary**: a collection of key and value pairs.
- **Exception**: an error Python raises at runtime.
- **Float**: a number with a decimal point.
- **Function**: a named, reusable block of code.
- **Index**: a position number in a string or list, starting at 0.
- **Integer**: a whole number.
- **List**: an ordered collection of items.
- **Loop**: code that repeats.
- **Module**: a file of reusable code.
- **Parameter**: a name in a function definition that receives a value.
- **String**: text in quotation marks.
- **Variable**: a name that stores a value.

## Final practice
1. Write a greeting program that asks for a name and prints a welcome.
2. Build a basic calculator that handles addition, subtraction, multiplication, and division.
3. Write an even-or-odd checker using a function.
4. Print a multiplication table from 1 to 10 using nested loops.
5. Create a simple quiz with a list of questions and answers, and score the user.
6. Write a text-file notes program that saves notes to a file.

## Common beginner mistakes
- Trying to learn everything at once. Revisit lessons when stuck.
- Skipping the exercises.

## Recap
You have covered variables, data types, input, operators, strings, conditions, loops, lists, dictionaries, functions, modules, errors, files, logic, and debugging.

## Challenge
Combine the calculator, the quiz, and the notes program into one menu-driven application.

## Example code

```python
# Lesson 20 example: a simple menu program combining earlier ideas

notes = []

def show_menu():
    print("\n1. Add a note")
    print("2. Show notes")
    print("3. Quit")

while True:
    show_menu()
    choice = input("Choose an option: ")

    if choice == "1":
        note = input("Type your note: ")
        notes.append(note)
        print("Note saved.")
    elif choice == "2":
        if len(notes) == 0:
            print("No notes yet.")
        for number, note in enumerate(notes, start=1):
            print(number, "-", note)
    elif choice == "3":
        print("Goodbye!")
        break
    else:
        print("Please choose 1, 2, or 3.")
```
