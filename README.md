# Exception Handling and JSON Module

A comprehensive Python guide and practical examples for file handling, exception handling, and working with JSON data.

## Overview

This repository contains educational materials and practical examples demonstrating:
- **File I/O Operations**: Reading and writing files in Python
- **Exception Handling**: Managing errors gracefully with try-except blocks
- **JSON Module**: Working with JSON data format for data serialization

## Contents

### Main Files

1. **File Handling and JSON Module.ipynb**
   - Jupyter notebook with comprehensive examples
   - Covers file operations (read, write, append, delete)
   - File modes explanation (r, w, a, x, b, t, +)
   - Exception handling mechanisms
   - List comprehension examples
   - JSON serialization and deserialization

2. **code.json**
   - Sample JSON data file
   - Contains user information: name, age, city, student status
   - Example:
     ```json
     {
       "name": "Ankit Mahato",
       "age": 20,
       "city": "Noida",
       "isStudent": true,
       "Address": {
         "city": "Noida",
         "state": "Uttar Pradesh"
       }
     }
     ```

3. **Sample Files** (sample.txt, sample1.txt, sample2.txt)
   - Text files for practicing file operations
   - Contains biographical and descriptive content

## Key Concepts

### File Operations
- **File Input (I)**: Reading data from files into your program
- **File Output (O)**: Writing data from your program into files
- **File Modes**:
  - `r` - Read mode (default)
  - `w` - Write mode (truncate file first)
  - `a` - Append mode (write at end)
  - `x` - Create and open for writing
  - `b` - Binary mode
  - `t` - Text mode (default)
  - `+` - Open disk file for update (read/write)

### Exception Handling
```python
try:
    # Code that might raise an exception
    result = 10 / x
except ZeroDivisionError:
    print("Cannot divide by zero!")
except ValueError:
    print("Please enter a valid number!")
else:
    print(f"Result is {result}")
finally:
    print("Execution completed.")
```

### JSON Module
- `json.loads()` - Convert JSON string to Python object
- `json.dumps()` - Convert Python object to JSON string
- `json.load()` - Read JSON from file
- `json.dump()` - Write JSON to file

## JSON-Python Data Type Mapping

| JSON | Python |
|------|--------|
| object | dict |
| array | list |
| string | str |
| number | int/float |
| true | True |
| false | False |
| null | None |

## Usage Examples

### Reading a File
```python
with open('sample.txt', 'r') as file:
    content = file.read()
    print(content)
```

### Working with JSON
```python
import json

# Loading JSON from file
with open('code.json', 'r') as file:
    data = json.load(file)
    print(data)

# Dumping to JSON file
with open('code.json', 'w') as file:
    json.dump(data, file, indent=4, sort_keys=True)
```

### Exception Handling with JSON
```python
try:
    with open('code.json', 'r') as file:
        data = json.load(file)
except FileNotFoundError:
    print("File not found!")
except json.JSONDecodeError:
    print("Invalid JSON format!")
```

## Learning Outcomes

After studying this repository, you will understand:
- ✓ How to read and write files in Python
- ✓ File modes and when to use each one
- ✓ Exception handling with try-except-finally blocks
- ✓ JSON data format and serialization
- ✓ Working with JSON files in Python
- ✓ Error handling best practices
- ✓ List comprehension techniques

## File Structure

```
Python/
├── README.md (this file)
├── File Handling and JSON Module.ipynb
├── code.json
├── sample.txt
├── sample1.txt
├── sample2.txt
└── exception_handling_and_json/
    └── example.py
```

## Requirements

- Python 3.7 or higher
- Jupyter Notebook (for running .ipynb files)
- No external dependencies required (uses built-in modules: json, os)

## Getting Started

1. Clone this repository or download the files
2. Open the Jupyter notebook to view detailed examples:
   ```bash
   jupyter notebook "File Handling and JSON Module.ipynb"
   ```
3. Review the sample JSON file to understand data structure
4. Experiment with the Python code examples

## Author

**Ankit Mahato**
- Location: Noida, Uttar Pradesh, India
- Contact: Via GitHub

## Topics Covered

- File I/O Operations
- Exception Handling
- Try-Except-Finally Blocks
- Error Management
- JSON Serialization
- List Comprehension
- Python 3.x Best Practices

## Notes

- The notebook uses Python 3.11.9
- All examples have been tested and executed
- Sample data includes personal information for demonstration purposes
- The repository is public and available for educational use

## Contributing

Feel free to fork this repository and add more examples or improvements!

---

**Last Updated**: January 2026
