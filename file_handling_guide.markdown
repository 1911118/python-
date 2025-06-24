# Simple File Handling in Python for Beginners

File handling lets you read, write, and manage files in Python. Below are easy, single-line commands with examples to get you started in Python IDLE.

## 1. Opening and Closing a File
- **Command**: `f = open("filename.txt", "mode")` - Opens a file in a mode like read ("r"), write ("w"), or append ("a").
- **Command**: `f.close()` - Closes the file to save resources.
- **Example**:
  ```python
  f = open("myfile.txt", "w")  # Open file to write
  f.close()  # Close the file
  ```

## 2. Common File Modes
- `"r"`: Read a file (default mode).
- `"w"`: Write to a file (creates or overwrites it).
- `"a"`: Append to a file (adds to the end).
- **Example**:
  ```python
  f = open("myfile.txt", "a")  # Open to append text
  f.close()
  ```

## 3. Reading a File
- **Command**: `f.read()` - Reads the entire file.
- **Command**: `f.readline()` - Reads one line.
- **Command**: `f.readlines()` - Reads all lines into a list.
- **Example**:
  ```python
  f = open("myfile.txt", "r")  # Open file to read
  print(f.read())  # Print all content
  f.close()
  ```

## 4. Writing to a File
- **Command**: `f.write("text")` - Writes text to the file.
- **Example**:
  ```python
  f = open("myfile.txt", "w")  # Open file to write
  f.write("Hello, Python!")  # Write text
  f.close()
  ```

## 5. Using "with" to Handle Files
- **Command**: `with open("filename.txt", "mode") as f:` - Opens and auto-closes the file.
- **Example**:
  ```python
  with open("myfile.txt", "w") as f:  # Open and write
      f.write("Easy file handling!")
  # File auto-closes after this
  ```

## 6. Simple File Operations
- **Command**: `import os; os.remove("filename.txt")` - Deletes a file.
- **Command**: `import os; os.rename("old.txt", "new.txt")` - Renames a file.
- **Example**:
  ```python
  import os
  os.rename("myfile.txt", "newfile.txt")  # Rename file
  ```

## Complete Example
```python
# Write to a file
with open("example.txt", "w") as f:
    f.write("Welcome to Python!")

# Read and print the file
with open("example.txt", "r") as f:
    print(f.read())  # Output: Welcome to Python!
```

Try these commands in Python IDLE to practice file handling!