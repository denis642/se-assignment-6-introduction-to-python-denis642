[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15276987&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Python is a high-level programming language known for its simplicity and readability. It is widely used in various domains such as web development, scientific computing, data analysis, artificial intelligence, and automation.

   Key Features of Python:
I.	Readability: Python's syntax is designed to be clear and readable, making it easier to write and maintain code.

II.	Versatility: It supports multiple programming paradigms, including procedural, object-oriented, and functional programming.

III.	Large Standard Library: Python comes with a vast collection of modules and libraries that facilitate tasks ranging from web development to scientific computing.

IV.	Community Support: Python has a large and active community, contributing to its rich ecosystem of libraries, frameworks, and resources.

V.	Interpreted and Interactive: Python is interpreted, allowing for quick development and testing. It also supports an interactive mode where you can test snippets of code.

VI.	Portability: Python code can run on various platforms and systems without modification.



2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Installing Python on Windows:

Download Python Installer:
Go to https://www.python.org/downloads/.
Download the latest version of Python for Windows.


Run the Installer:
Run the downloaded installer (python-3.x.x.exe).
Check the box "Add Python x.x to PATH" during installation.


Verify Installation:
Open Command Prompt (cmd).
Type python --version or python -V to check the installed Python version.


Setting Up a Virtual Environment:
Install virtualenv:
Open Command Prompt (cmd).
Install virtualenv using pip

Create a Virtual Environment:

mkdir myproject
cd myproject
python -m venv venv


Activate the Virtual Environment:

In the Command Prompt, navigate to your project directory.
Activate the virtual environment:
venv\Scripts\activate
Verify Virtual Environment:

You should see (venv) at the beginning of your command prompt.

Install packages with pip which will be isolated to this environment.

3. Python Syntax and Semantics:
   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

 Simple Python program to print Hello, World!

print("Hello, World!")

Comments (#):

Comments in Python start with a hash (#) symbol and are used to annotate code. They are ignored by the Python interpreter and are helpful for documenting code or temporarily disabling parts of code.

Print Statement (print()):

The print() function in Python is used to output text or variables to the console (standard output). In this case, "Hello, World!" is passed as an argument to print().

String Literal ("Hello, World!"):

"Hello, World!" is a string literal in Python. String literals are sequences of characters enclosed within double quotes ("). They can also be enclosed in single quotes (') with the same effect.

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Basic Data Types in Python:
Integer (int):

Represents whole numbers, both positive and negative.
Example: x = 5
Float (float):

Represents floating-point numbers, which include decimals.
Example: y = 3.14
String (str):

Represents sequences of characters enclosed within quotes (" or ').
Example: name = "Alice"
Boolean (bool):

Represents a value of either True or False.
Example: is_valid = True
List (list):

Represents an ordered collection of items, which can be of different types.
Example: numbers = [1, 2, 3, 4]
Tuple (tuple):

Similar to lists, but tuples are immutable (cannot be changed after creation).
Example: coordinates = (3, 4)
Dictionary (dict):

Represents a collection of key-value pairs where each key is associated with a value.
Example: person = {'name': 'Bob', 'age': 30}


example of a script to show the above.


x = 5                   # integer


y = 3.14                # float


name = "Alice"          # string


is_valid = True         # boolean



numbers = [1, 2, 3, 4]  # list


coordinates = (3, 4)    # tuple


person = {'name': 'Bob', 'age': 30}  # dictionary


To Print the variables and their types:


print(f"Variable x: {x}, Type: {type(x)}")


print(f"Variable y: {y}, Type: {type(y)}")


print(f"Variable name: {name}, Type: {type(name)}")


print(f"Variable is_valid: {is_valid}, Type: {type(is_valid)}")


print(f"Variable numbers: {numbers}, Type: {type(numbers)}")


print(f"Variable coordinates: {coordinates}, Type: {type(coordinates)}")


print(f"Variable person: {person}, Type: {type(person)}")




5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Conditional Statements (if-else):
Conditional statements are used to make decisions based on conditions. In Python, the if-else statement is the most basic form of conditional execution.

example:

Example 1: Checking if a number is positive or negative

num = 10


if num >= 0:
    print(f"{num} is a positive number.")


else:
    print(f"{num} is a negative number.")




Loops (for loop):

Loops in Python allow you to repeatedly execute a block of code. The for loop is used to iterate over a sequence (such as a list, tuple, or string) or other iterable objects.

example:


 Example 2: Iterating over a list of names and printing each name


names = ["Alice", "Bob", "Charlie", "David"]


for name in names:
    print(f"Hello, {name}!")



6. Functions in Python:
   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.


   Functions in Python are blocks of organized, reusable code that perform a specific task. They provide modularity to a program by breaking it into smaller, manageable pieces. Functions are defined using the def keyword, and they can accept parameters, perform actions, and optionally return a value.

Key Benefits of Functions:
Modularity: Functions allow you to break down complex tasks into smaller, more manageable tasks, improving code readability and maintainability.

Code Reusability: Once defined, functions can be called multiple times from different parts of the program without duplicating code.

Abstraction: Functions hide the implementation details of their logic, allowing you to focus on what a function does rather than how it does it.

Ease of Testing and Debugging: Functions make it easier to test individual parts of your code and isolate errors.

example:

 Define a function that takes two arguments and returns their sum


def calculate_sum(a, b):


    return a + b


 Example of how to call this function


result = calculate_sum(3, 5)


print(f"The sum is: {result}")


7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

I.	Lists are ordered collections of items while Dictionaries are unordered collections of key-value pairs.

II.	Elements in a list are accessed by their position (index) while Elements in a dictionary are accessed using keys rather than indexes.

III.	Defined with square brackets [ ] while dictionaries defined with curly braces { }, with each item being a key: value pair

example:


 a list of numbers:


numbers = [1, 2, 3, 4, 5]


 a dictionary of key-value pairs


person = {

    "name": "Alice",


    "age": 30,


    "city": "New York",


    "email": "alice@example.com"
}


 to Print the original list and dictionary


print("Original list of numbers:", numbers)


print("Original dictionary:", person)


print()

Accessing elements:

print("Accessing elements:")

print("Third number in the list:", numbers[2])

print("Age of the person:", person["age"])

print()


 Modifying elements:

numbers[0] = 10

person["city"] = "San Francisco"

print("Modified list after changing first element:", numbers)

print("Modified dictionary after changing city:", person)

print()


 Adding elements:

numbers.append(6)

person["phone"] = "123-456-7890"

print("List after appending a number:", numbers)

print("Dictionary after adding a phone number:", person)

print()

Removing elements:


numbers.pop()

del person["email"]

print("List after removing the last element:", numbers)

print("Dictionary after deleting email:", person)



8. Exception Handling:
   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Exception handling in Python allows you to handle runtime errors gracefully, preventing your program from crashing when unexpected situations occur. It involves using try, except, and optionally finally blocks to catch and handle exceptions.

   example:

    Example of exception handling with try, except, and finally blocks

def divide_numbers(a, b):

    try:
        result = a / b

    except ZeroDivisionError:

        print("Error: Division by zero!")

    except TypeError:

        print("Error: Unsupported operand type(s) for division!")

    else:

        print(f"The result of {a} divided by {b} is: {result}")

    finally:

        print("Executing finally block. Clean up resources here if needed.")

An Example usage:

divide_numbers(10, 2)   # Normal division

divide_numbers(10, 0)   # Division by zero exception

divide_numbers(10, '2') # Type error exception


9. Modules and Packages:
   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   Modules in Python are files containing Python code. They can define functions, classes, and variables that can be reused in other Python scripts.

   Packages are namespaces that contain multiple modules and sub-packages. They provide a way of structuring Python’s module namespace by using "dotted module names".

Importing and Using Modules in Python:
To use a module in Python, you typically import it into your script using the import statement.

Example using the math module


import math

print(math.sqrt(25))    # Output: 5.0 (square root of 25)

print(math.floor(5.7))  # Output: 5 (floor of 5.7)

print(math.pi)          # Output: 3.141592653589793 (value of pi)


 Importing specific functions and constants from the math module:

from math import factorial, radians


 Using the imported functions directly:

print(factorial(5))     # Output: 120 (factorial of 5)

print(radians(90))      # Output: 1.5707963267948966 (radians equivalent of 90 degrees)


Aliasing the math module:

import math as m


 Using an alias to access module functions:

print(m.cos(m.pi))      # Output: -1.0 (cosine of pi)



10. File I/O:
    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

To read from a file in Python:

Open the File: Use the open() function with the file path and mode ('r' for reading) to open the file.
Read the Content: Use methods like read(), readline(), or readlines() to read the file content.
Close the File: Always close the file using the close() method to free up system resources.

 Example: Reading from a file and printing its content


file_path = 'example.txt'

try:

    with open(file_path, 'r') as file:

        # Read and print the entire content

        content = file.read()

        print("Content of the file:")

        print(content)

except FileNotFoundError:

    print(f"Error: The file '{file_path}' does not exist.")

except IOError:

    print(f"Error: Could not read from the file '{file_path}'.")




 Example: Writing a list of strings to a file


lines = [

    "Hello, this is line 1.",

    "This is line 2.",

    "And this is line 3."
]


A File path where we want to write:

file_path = 'output.txt'


try:

    # Open the file in write mode

    with open(file_path, 'w') as file:

        # Write each line from the list to the file

        for line in lines:

            file.write(line + '\n')

    print(f"Successfully wrote {len(lines)} lines to '{file_path}'.")

except IOError:

    print(f"Error: Could not write to the file '{file_path}'.")
    


# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].


