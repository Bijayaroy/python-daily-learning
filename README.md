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
## Day 10: More Functions for Array
Some more useful functions provided in Python for arrays:

### Array Typecode Function
This function returns the data type by which the array is initialized. In this example, we are using arr.typecode to find out the data type of array initialization.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr= array.array('i',[1, 2, 3, 1, 2, 5]) 
   
# using typecode to print datatype of array
print ("The datatype of array is : ")
print (arr.typecode)
#Output

#The datatype of array is : 
#i
```

### Array itemsize Function
This function returns the size in bytes of a single array element. In this example, we are using itemsize function to find out the size in byte of an array element.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr= array.array('i',[1, 2, 3, 1, 2, 5]) 
   
# using itemsize to print itemsize of array
print ("The itemsize of array is : ")
print (arr.itemsize)
#Output
#The itemsize of array is : 
#4
```

### buffer_info() in Python
Returns a tuple representing the address in which array is stored and number of elements in it. In this example, we are using buffer_info() to do the same.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr= array.array('i',[1, 2, 3, 1, 2, 5]) 
 
# using buffer_info() to print buffer info. of array
print ("The buffer info. of array is : ")
print (arr.buffer_info())
#Output
#The buffer info. of array is : 
#(140491260368688, 6)
```

### Array fromlist() Function
This function is used to append a list mentioned in its argument to end of array. In this example, we are using fromlist() to append a list to end of array.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr = array.array('i',[1, 2, 3, 1, 2, 5]) 
li = [1, 2, 3]
   
# using fromlist() to append list at end of array
arr.fromlist(li)
   
# printing the modified array
print ("The modified array is : ",end="")
for i in range (0,9):
    print (arr[i],end=" ")
#Output
#The modified array is : 1 2 3 1 2 5 1 2 3 
```

### tolist() in Python
This function is used to transform an array into a list. In this example, we are using tolist() to convert an array to list.

```python
# importing "array" for array operations
import array
    
# initializing array with array values
arr = array.array('i',[1, 2, 3, 1, 2, 5]) 
   
# using tolist() to convert array into list
li2 = arr.tolist()
   
# printing the new list
print ("The new list created is : ",end="")
for i in range (0,len(li2)):
    print (li2[i],end=" ")
#Output
#The new list created is : 1 2 3 1 2 5 
```
# Day 11: Strings
In Python, a string is a sequence of characters enclosed within single quotes (' '), double quotes (" "), or triple quotes (''' ''' or """ """). 

Strings are immutable, meaning that once they are created, their values cannot be changed.
Like many other popular programming languages, strings in Python are arrays of bytes representing unicode characters.
However, Python does not have a character data type, a single character is simply a string with a length of 1.
Square brackets can be used to access elements of the string.
```python
a = "Hello, World!"
print(a[1])
```
Assigning a string to a variable is done with the variable name followed by an equal sign and the string:
```python
a = "Hello"
print(a)
```
Python provides a variety of built-in methods for manipulating strings. Some commonly used methods include:

- len(string): Returns the length of the string.
- string.lower(), string.upper(): Converts the string to lowercase or uppercase.
- string.startswith(prefix), string.endswith(suffix): Checks if the string starts or ends with a specified prefix or suffix.
- string.find(substring): Returns the index of the first occurrence of the substring, or -1 if not found.

# Day 12: Strings(contd.)
More functions related to it:
string.strip(), string.lstrip(), string.rstrip(): Removes any whitespaces before or at the end.
```python
sentence = "   This is a sample sentence.   "
print(sentence.strip())
# Output: "This is a sample sentence."
```
Check String: To check if a certain phrase or character is present in a string, we can use the keyword in.
```python
txt = "The best things in life are free!"
print("free" in txt)

text = "The best things in life are free!"
print("expensive" not in text)
```
Slicing: You can return a range of characters by using the slice syntax. Specify the start index and the end index, separated by a colon, to return a part of the string.
```python
b = "Hello, World!"
print(b[2:5])
```
Replace String: The replace() method replaces a string with another string:
```python
a = "Hello, World!"
print(a.replace("H", "J"))
```
Split String: The split() method returns a list where the text between the specified separator becomes the list items.
```python
a = "Hello, World!"
print(a.split(",")) # returns ['Hello', ' World!']
```
# Day 13 : Numpy array

NumPy arrays are a fundamental data structure in the NumPy library, which is a popular Python library used for numerical computing. NumPy arrays provide a way to store and manipulate large arrays of numerical data efficiently.

Here's a brief overview of NumPy arrays:

Homogeneous Data: NumPy arrays are homogeneous, meaning all elements in the array must have the same data type. This contrasts with Python lists, which can contain elements of different data types.

Multidimensional: NumPy arrays can have any number of dimensions. The most common are 1-dimensional arrays (vectors), 2-dimensional arrays (matrices), and higher-dimensional arrays.

Efficiency: NumPy arrays are implemented in C, which makes them much more efficient than Python lists, especially for large datasets.

Universal Functions (ufuncs): NumPy provides a large set of mathematical functions that operate element-wise on arrays, known as universal functions or ufuncs. These functions allow for fast computations on arrays without the need for explicit looping in Python.

Indexing and Slicing: NumPy arrays support advanced indexing and slicing operations, similar to Python lists, allowing you to access subsets of the array efficiently.

Broadcasting: NumPy arrays support broadcasting, which is a powerful mechanism that allows arithmetic operations to be performed between arrays of different shapes, often eliminating the need for explicit looping.

Integration with other Libraries: NumPy arrays are used as the standard data structure for exchanging data between different scientific computing libraries in Python, such as SciPy, Pandas, Matplotlib, and scikit-learn.

Here's a simple example of creating a NumPy array and performing some basic operations:

```python
import numpy as np

# Creating a 1-dimensional NumPy array
arr1d = np.array([1, 2, 3, 4, 5])

# Creating a 2-dimensional NumPy array
arr2d = np.array([[1, 2, 3], [4, 5, 6]])

# Accessing elements of an array
print(arr1d[0])  # Output: 1
print(arr2d[1, 2])  # Output: 6

# Slicing arrays
print(arr1d[:3])  # Output: [1 2 3]
print(arr2d[:, 1:])  # Output: [[2 3]
                      #          [5 6]]

# Performing arithmetic operations
result = arr1d * 2
print(result)  # Output: [ 2  4  6  8 10]

# Broadcasting
arr3 = np.array([[1], [2], [3]])
arr4 = np.array([1, 2, 3])
result = arr3 + arr4
print(result)  # Output: [[2 3 4]
               #          [3 4 5]
               #          [4 5 6]]
```
0-D Arrays
0-D arrays, or Scalars, are the elements in an array. Each value in an array is a 0-D array.

```python
import numpy as np

arr = np.array(42)

print(arr)
```
1-D Arrays
An array that has 0-D arrays as its elements is called uni-dimensional or 1-D array.

These are the most common and basic arrays.
```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])

print(arr)
```
2-D Arrays
An array that has 1-D arrays as its elements is called a 2-D array.

These are often used to represent matrix or 2nd order tensors.

NumPy has a whole sub module dedicated towards matrix operations called numpy.mat

```python
import numpy as np

arr = np.array([[1, 2, 3], [4, 5, 6]])

print(arr)
```
3-D arrays
An array that has 2-D arrays (matrices) as its elements is called 3-D array.

These are often used to represent a 3rd order tensor.

```python
import numpy as np

arr = np.array([[[1, 2, 3], [4, 5, 6]], [[1, 2, 3], [4, 5, 6]]])

print(arr)
```
NumPy Arrays provides the [ndim] attribute that returns an integer that tells us how many dimensions the array have.
Negative Indexing
Use negative indexing to access an array from the end.

```python
import numpy as np

arr = np.array([[1,2,3,4,5], [6,7,8,9,10]])

print('Last element from 2nd dim: ', arr[1, -1])
```
Data Types in NumPy
NumPy has some extra data types, and refer to data types with one character, like i for integers, u for unsigned integers etc.

Below is a list of all data types in NumPy and the characters used to represent them.

i - integer
b - boolean
u - unsigned integer
f - float
c - complex float
m - timedelta
M - datetime
O - object
S - string
U - unicode string
V - fixed chunk of memory for other type ( void )

Change data type from float to integer by using 'i' as parameter value:
```python
import numpy as np

arr = np.array([1.1, 2.1, 3.1])

newarr = arr.astype('i')

print(newarr)
print(newarr.dtype)
```

### Hackerrank Challenge: 
Q1.The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students. Print the average of the marks array for the student name provided, showing 2 places after the decimal.

```python
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    
    if query_name in student_marks:
        marks = student_marks[query_name]
        average = sum(marks) / len(marks)
        print("{:.2f}".format(average))
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/53acd6a5-872a-4c89-9bb7-c16e1804b154)

Q2. You are given a two lists A and B. Your task is to compute their cartesian product X.

```python
# Take user input for the first list
list1 = input().split()

# Take user input for the second list
list2 = input().split()

# Convert elements to integers
list1 = [int(x) for x in list1]
list2 = [int(x) for x in list2]

# Using list comprehension to compute Cartesian product
cartesian_product = [(x, y) for x in list1 for y in list2]

# Printing each tuple separately
for pair in cartesian_product:
    print(pair, end=" ")
```
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e699cf29-aeda-48f1-b792-24800596ed7d)
