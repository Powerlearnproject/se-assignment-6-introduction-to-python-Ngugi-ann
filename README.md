[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15299258&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
   Python is a high-level, interpreted programming language known for its readability, simplicity, and versatility.
   Key Features of Python:
Readability and Simplicity: Python's syntax is clean and easy to understand, which reduces the learning curve for beginners and increases productivity for experienced developers.
Extensive Standard Library: Python comes with a vast standard library that supports many common programming tasks, from file I/O to web development and beyond.
Cross-Platform Compatibility: Python runs on various platforms, including Windows, macOS, and Linux, without requiring changes to the code.
Dynamic Typing: Variables in Python are dynamically typed, meaning you don't have to declare their type explicitly.
Interpreted Language: Python code is executed line by line, which makes debugging easier and accelerates development.
Web Development: Frameworks like Django and Flask make it easy to build robust and scalable web applications.

Example: Django, a high-level web framework, allows rapid development and clean, pragmatic design.
Data Science and Machine Learning: Libraries such as Pandas, NumPy, and Scikit-learn are widely used for data analysis, manipulation, and machine learning.

Example: Jupyter Notebooks are often used for data analysis and visualization, combining code, text, and graphics.


2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   Windows:
Download the Python installer from the official website.
Run the installer and check "Add Python to PATH".
Click "Install Now".
Verifying the Installation:

Open a terminal or command prompt.
Run: python --version or python3 --version.
Setting Up a Virtual Environment:

Install virtualenv if not already installed: pip install virtualenv.
Navigate to your project directory.
Create a virtual environment: python -m venv venv (or python3 -m venv venv).
Activate the virtual environment:
Windows: .\venv\Scripts\activate

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.
   python
print("Hello, World!")

Basic Syntax Elements:
print(): A built-in Python function that outputs text to the console.
"Hello, World!": A string (a sequence of characters) enclosed in double quotes. The text inside the quotes is what will be printed.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
   Basic Data Types in Python
Integer (int): Whole numbers, positive or negative, without decimals. Example: 44
Float (float): Numbers with decimals. Example: 2.14
String (str): Sequence of characters enclosed in quotes. Example: "Hello"
Boolean (bool): Represents True or False.
List (list): Ordered, mutable collection of items. Example: [1, 2, 3]
Tuple (tuple): Ordered, immutable collection of items. Example: (1, 2, 3)
Dictionary (dict): Unordered collection of key-value pairs. Example: {"key": "value"}
Set (set): Unordered collection of unique items. Example: {1, 2, 3}
Short Script Demonstrating Basic Data Types
python
# Integer
my_int = 42
print("Integer:", my_int)

# Float
my_float = 3.14
print("Float:", my_float)

# String
my_str = "Hello, World!"
print("String:", my_str)

# Boolean
my_bool = True
print("Boolean:", my_bool)

# List
my_list = [1, 2, 3, 4]
print("List:", my_list)

# Tuple
my_tuple = (1, 2, 3, 4)
print("Tuple:", my_tuple)

# Dictionary
my_dict = {"name": "Alice", "age": 30}
print("Dictionary:", my_dict)

# Set
my_set = {1, 2, 3, 4}
print("Set:", my_set)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
   Conditional Statements
Conditional statements in Python allow you to execute specific code blocks based on certain conditions.
if statement: Executes a block of code if the condition is true.
else statement: Executes a block of code if the condition in the if statement is false.
elif (else if): Checks another condition if the previous conditions were false.

Example of if-else statement:
python
age = 18
if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
Loops
Loops in Python allow you to execute a block of code multiple times.
for loop: Iterates over a sequence (like a list, tuple, or string) and executes a block of code for each item.

Example of for loop:
python
numbers = [1, 2, 3, 4, 5]
for number in numbers:
    print(number)

6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
   Functions in Python are reusable blocks of code that perform specific tasks. They help to organize your code, make it more readable, and avoid repetition.

Here's a Python function named sum_numbers that takes two arguments (x and y) and returns their sum:
Python
def sum_numbers(x, y):
  """This function takes two numbers as arguments and returns their sum."""
  return x + y

# Example call to the function
result = sum_numbers(5, 3)
print(result)  # Output: 8

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
   In Python, lists and dictionaries are two fundamental data structures with key differences:
Lists are ordered collections of items. They are created using square brackets [] and can contain elements of different data types. Elements in a list are accessed by their index, starting from 0.
Dictionaries are unordered collections of key-value pairs. They are created using curly braces {} and each element in a dictionary is accessed by its key.
# Create a list of numbers
numbers = [1, 2, 3, 4, 5]

# Create a dictionary with some key-value pairs
person = {
    'name': 'Alice',
    'age': 30,
    'city': 'Nairobi'
}

# Accessing elements
print(numbers[0])          # Output: 1
print(person['name'])      # Output: Alice


8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.
   Exception handling in Python allows you to manage errors that occur during program execution. You use try to wrap the code that might raise an exception, except to handle specific exceptions, and finally to execute code regardless of whether an exception occurred.

python
try:
    # Code that might raise an exception
    result = 10 / 0
except ZeroDivisionError:
    # Handle the specific exception
    print("Division by zero is not allowed.")
finally:
    # Code that will always execute
    print("Execution complete.")

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.
   Modules in Python are files containing Python code. They can define functions, classes, and variables. Python modules have a .py extension and can be imported into other Python scripts or modules using the import keyword.

Packages in Python are directories containing multiple modules. Each package directory contains a special file called __init__.py, which indicates that the directory should be treated as a package.

To import a module in Python, you use the import keyword followed by the module name. For example, to import the math module, you would use:

python
import math
You can then use functions and variables defined in the math module by prefixing them with math.. For example:

python
import math

# Calculate the square root of 16
sqrt = math.sqrt(16)
print(sqrt)  # Output: 4.0

10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.
    Reading from files: You can read from a file in Python using the open() function to open a file in read mode ('r'). Then, you can use methods like read(), readline(), or readlines() to read the contents of the file.

Writing to files: To write to a file in Python, you can open a file in write mode ('w') using the open() function. You can then use the write() method to write to the file.

Here's an example script that reads the content of a file and prints it to the console:

python
# Open a file in read mode
with open('example.txt', 'r') as file:
    # Read the entire file content
    content = file.read()
    # Print the content to the console
    print(content)
And here's an example script that writes a list of strings to a file:

python
# List of strings
lines = ['Line 1\n', 'Line 2\n', 'Line 3\n']

# Open a file in write mode
with open('output.txt', 'w') as file:
    # Write each string in the list to the file
    file.writelines(lines)

# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


