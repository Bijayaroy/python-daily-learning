# PYTHON 
## Day 1: Introduction to Python

- History of Python:
  - Python was created by Guido van Rossum and first released in 1991.
  - Python's story begins in December 1989 when Guido van Rossum, a Dutch programmer, started working on a new programming language during his Christmas holidays. Van Rossum's goal was to create a language that would emphasize code readability and encourage developers to write clean and expressive code.
- One of the most important changes in Python's evolution has been the addition of new libraries and frameworks. These libraries provide pre-written code that can be used to perform common tasks, such as accessing databases, sending emails, and creating web applications. This has made Python even more powerful and versatile, and has helped it to become one of the most popular programming languages in the world.

- Basic Introduction:
  - Python is a high-level, interpreted programming language. This means that Python code is easy for humans to read and write, and it does not need to be compiled before it can be run. Python is also interpreted, which means that it is executed one line at a time, as it is read by the interpreter. Python is a general-purpose programming language, which means that it can be used for a wide variety of tasks, including web development, data science, machine learning, and more. Python is also a very popular language for beginners, as it is relatively easy to learn and use

## Day 2: Understanding Python Syntax
Indentation:
Python uses indentation to define blocks of code. This means that all lines of code that belong to the same block must be indented at the same level.


White space:
Python uses white space to separate different elements of a code statement. This includes spaces, tabs, and newlines.


Keywords:
Keywords are special words that have a specific meaning in Python. They cannot be used as variable names.


Identifiers:
Identifiers are used to name variables, functions, classes, and other objects in Python. They must start with a letter or an underscore (_) and can contain letters, numbers, and underscores.


Operators:
Operators are used to perform operations on data. They include arithmetic operators, comparison operators, logical operators, and assignment operators.


Comments:
Comments are important for code readability because they make it easier for other developers to understand your code. When you write comments, you are essentially explaining your code to yourself and others. This can be helpful when you are working on a project with other people, or when you come back to your code later and need to remember what it does.
There are three different types of comments in Python:
Single-line comments: These comments start with a hash (#) and continue to the end of the line.
Multi-line comments: These comments start with a triple quote (""") and end with a triple quote.

## Day 3: Variables and Data Types

### Variables:
  - Variables are used to store and manage data in a program.
```python
age = 25
name = "John"
```
Variable naming conventions and best practices:
use lowercase with underscores for readability.
Descriptive and meaningful names enhance code clarity.
```python
user_age = 25
user_name = "John"
```
### Data Types:
  - Fundamental data types: int, float, str, bool.
int: Represents integers.
float: Represents floating-point numbers.
str: Represents strings.
bool: Represents Boolean values (True or False).

```python
age = 25 # int
height = 5.9 # float
name = "John" # str
is_adult = True # bool
```
Exploring their characteristics and use cases.
```python
x = 5 + 2.0      # Results in a float
message = "Hello, " + "world!"  # String concatenation
```

## Day 4 : Conditional Statements (if, elif, else) and Numbers, Casting, and Operators:
### (if, elif, else):
Control the flow of a program based on conditions.
```python
x = 10

if x > 0:
 print("Positive")
elif x == 0:
 print("Zero")
else:
 print("Negative")
```
### Numbers, Casting, and Operators:

- Numbers:
  - Working with integers and floats.
```python
x = 5
y = 2.0
sum_result = x + y
```

- Casting and Type Conversion:
	Changing the data type of a variable.
```python
x = 5.7
int_x = int(x)  # Casting to int, result: 5
```

  - Method for converting between data types.
	Use functions like int(), float(), str(), etc.

- Operators:
  - Exploring arithmetic, comparison, logical, and assignment operators like +, -, *, /, ==, !=, and, or, +=, etc.
Example:
```python
result = (3 + 4) * 2 # Arithmetic
is_equal = (x == y) # Comparison
```

## Day 5 : Loops (for, while):
### For Loop:
```python
for i in range(5):
 print(i)
```
### While Loop:
```python
i = 0
while i < 5:
 print(i)
 i += 1
```
### Break and Continue Statements:
Break:
```python
for i in range(10):
 if i == 5:
 break
 print(i)
```
Continue:
```python
for i in range(10):
 if i == 5:
 continue
print(i)
```
## Day 6 : Functions
### Functions:
A function is a block of organized, reusable code that performs a specific task.
Functions help in modularizing code and promoting reusability.

Syntax:
```python
def function_name(parameters):
    # Function body
    # ...
    return result  # optional
```
Example:

```python
def greet(name):
    return f"Hello, {name}!"

result = greet("John")
print(result)
```


### Parameters and Arguments:

Parameters are variables in a function definition.
Arguments are values passed into a function.


### Return Statement:

A function can return a value using the return statement.
If no return statement is present, the function returns None by default.


### Scope:

Variables defined inside a function are local to that function.
Variables defined outside functions are global.

## Day 7: Modular Programming:
### Modular Programming:
Modular programming is a software design technique where a program is divided into independent, interchangeable modules.
Advantages:

Reusability: Modules can be reused in different parts of the program.
Maintainability: Changes in one module don't affect others if the interface remains the same.
Scalability: Easier to scale by adding or removing modules.
How to Create Modules:

Save a Python script (.py file) with functions and variables.
Import the module into another script using import module_name.
Example Module (math_operations.py):

```python
# math_operations.py
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y
```
Using the Module in Another Script:

```python
# main_script.py
import math_operations

result_add = math_operations.add(5, 3)
result_subtract = math_operations.subtract(8, 4)

print(result_add, result_subtract)
```
### if name == "main":

Allows a script to be used both as an importable module and as a standalone script.
```python
# math_operations.py
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

if __name__ == "__main__":
    # Code only executed when the script is run directly
    print(add(5, 3))
```
## Day 8: Arrays
In Python, arrays are often implemented using the built-in list type. The array can also be handled in Python by a module named array. They can be useful when we have to manipulate only specific data type values. A user can treat lists as arrays. However, the user cannot constrain the type of elements stored in a list. If you create arrays using the array module, all elements of the array must be of the same type.  While Python doesn't have a native array type like some other programming languages, its lists provide dynamic arrays with additional functionalities. (Source: GeeksForGeeks)

### Arrays (using Python Lists):
Creation:
```python
my_array = [1, 2, 3, 4, 5]
```
### Adding Elements:

You can use append() to add elements to the end of the array.
```python
my_array.append(6)
```
### Removing Elements:

Use .pop() or .remove() to remove and return an element by index.
```python
removed_element = my_array.pop(2)
```
### Indexing and Slicing:

Slice operation is performed on array with the use of colon(:). To print elements from beginning to a range use [:Index], to print elements from end use [:-Index], to print elements from specific Index till the end use [Index:], to print elements within a range, use [Start Index:End Index] and to print whole List with the use of slicing operation, use [:]. Further, to print whole array in reverse order, use [::-1].
```python
sublist = my_list[1:4]  # Elements from index 1 to 3
```
Common Operations:

Find the index of an element: my_array.index(element).
Count occurrences of an element: my_array.count(element).


NumPy Arrays:
If you need more advanced array manipulation and operations, you can use the NumPy library, which provides efficient and convenient array-like objects.

Installation:

`
pip install numpy
`


Creating NumPy Arrays:

```python
import numpy as np
numpy_array = np.array([1, 2, 3, 4, 5])
```
Operations:

NumPy allows element-wise operations and supports a variety of mathematical operations directly on arrays.
```python
result_array = numpy_array * 2
```
### Array Manipulation:

Reshaping: numpy_array.reshape(rows, columns).
Concatenation: np.concatenate((array1, array2)).
 
Similar to Python lists but extended for multi-dimensional arrays.
```python
squared_array = [x**2 for x in range(1, 6)]
```
Important Note:
- NumPy arrays are more efficient for numerical computations compared to Python lists, especially for large datasets.
- When dealing with mathematical and scientific computations involving arrays, NumPy is the preferred choice due to its optimized implementations.

## Day 9 : Programs related to Array:

### Printing an array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [1, 2, 3, 4, 5])

# print the array
print(numbers)

# Output: array('i', [1, 2, 3, 4, 5])
```
### Finding the largest number in an array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [10, 5, 15, 4, 6, 20, 9])

# find the largest number
largest = numbers[0]
for i in range(1, len(numbers)):
    if numbers[i] > largest:
        largest = numbers[i]

# print the largest number
print("Largest number:", largest)

# Output: Largest number: 20
```
### Sum of elements in an array:
```python
def sum(arr):
    result = 0
    for x in arr:
        result += x
    return result
```
### Storing all even numbers from an array in another array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [10, 5, 15, 4, 6, 20, 9])

# create an empty array to store even numbers
even_numbers = arr.array('i', [])

# iterate over the original array and add even numbers to the new array
for number in numbers:
    if number % 2 == 0:
        even_numbers.append(number)

# print the new array
print(even_numbers)

# Output: array('i', [10, 4, 6, 20])
```
### Finding the average of all numbers in an array:
```python
import array as arr

# create an array of integers
numbers = arr.array('i', [1, 2, 3, 4, 5])

# calculate the sum of all numbers
sum = 0
for number in numbers:
    sum += number

# calculate the average
average = sum / len(numbers)

# print the average
print("Average:", average)

# Output: Average: 3.0
```
