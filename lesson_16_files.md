# Lesson 16: Files

## Reading and writing text files
Use `with open()` so Python closes the file automatically, even if an error happens.

    with open("notes.txt", "w") as file:
        file.write("First line\n")

Mode letters: `"w"` writes (replaces the file), `"a"` appends to the end, `"r"` reads.

## Reading
    with open("notes.txt", "r") as file:
        content = file.read()
        print(content)

## Handling a missing file
    try:
        with open("missing.txt") as file:
            print(file.read())
    except FileNotFoundError:
        print("The file does not exist yet.")

## Practice exercises
1. Write a sentence to `diary.txt`.
2. Append a second sentence to the same file.
3. Read the file and print it.

## Common beginner mistakes
- Using `"w"` by accident, which erases existing content.
- Forgetting `\n` to start a new line.

## Recap
- `with open()` handles files safely.
- Choose `"r"`, `"w"`, or `"a"` carefully.

## Challenge
Build a notes program that adds a line each time the user types a note, and shows all notes on request.

## Example code

```python
# Lesson 16 example: files

# Write a file (this replaces anything already in it)
with open("example_notes.txt", "w") as file:
    file.write("First note\n")

# Append another line to the end
with open("example_notes.txt", "a") as file:
    file.write("Second note\n")

# Read the whole file back
with open("example_notes.txt", "r") as file:
    print(file.read())

# Handle a missing file safely
try:
    with open("does_not_exist.txt") as file:
        print(file.read())
except FileNotFoundError:
    print("That file does not exist.")
```
