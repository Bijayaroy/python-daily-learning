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
## Day 11: Strings
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
## Day 13 : Numpy array

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

## Day 14: Tree
A tree represents hierarchical relationships between elements. It consists of nodes connected by edges. Each node contains a value (or data) and references to its child nodes. The topmost node in a tree is called the root node, and nodes with no children are called leaf nodes.

The Tree data structure can be useful in many cases:

Hierarchical Data: File systems, organizational models, etc.
Databases: Used for quick data retrieval.
Routing Tables: Used for routing data in network algorithms.
Sorting/Searching: Used for sorting data and searching for data.

Tree Terminology and Rules:

- The first node in a tree is called the root node.
- A link connecting one node to another is called an edge.
- A parent node has links to its child nodes. Another word for a parent node is internal node.
- A node can have zero, one, or many child nodes.
- A node can only have one parent node.
- Nodes without links to other child nodes are called leaves, or leaf nodes.
- The tree height is the maximum number of edges from the root node to a leaf node. The height of the tree above is 2.
- The height of a node is the maximum number of edges between the node and a leaf node.
- The tree size is the number of nodes in the tree.

Types of Trees
- Binary Trees: Each node has up to two children, the left child node and the right child node. This structure is the foundation for more complex tree types like Binary Search Trees and AVL Trees.
- Binary Search Trees (BSTs): A type of Binary Tree where for each node, the left child node has a lower value, and the right child node has a higher value.
- AVL Trees: A type of Binary Search Tree that self-balances so that for every node, the difference in height between the left and right subtrees is at most one. This balance is maintained through rotations when nodes are inserted or deleted.

A binary tree is a hierarchical data structure composed of nodes, where each node has at most two children, referred to as the left child and the right child. The topmost node of the tree is called the root node. In a binary tree, each child node can have a reference to its parent node.

Benefits of Binary Trees over Arrays and Linked Lists:

Arrays are fast when you want to access an element directly, like element number 700 in an array of 1000 elements for example. But inserting and deleting elements require other elements to shift in memory to make place for the new element, or to take the deleted elements place, and that is time consuming.
Linked Lists are fast when inserting or deleting nodes, no memory shifting needed, but to access an element inside the list, the list must be traversed, and that takes time.
Binary Trees, such as Binary Search Trees and AVL Trees, are great compared to Arrays and Linked Lists because they are BOTH fast at accessing a node, AND fast when it comes to deleting or inserting a node, with no shifts in memory needed.

Properties of Binary Trees:
Root Node: The topmost node in a binary tree.
Parent Node: A node that has child nodes.
Child Node: A node that is connected to a parent node.
Leaf Node: A node that does not have any children.
Internal Node: A node that has at least one child.
Height: The height of a binary tree is the maximum distance from the root node to a leaf node. The height of an empty tree is considered to be -1.
Depth (or Level): The depth of a node is the number of edges from the root node to that node.
Balanced Binary Tree: A binary tree in which the heights of the left and right subtrees of any node differ by at most one.
Complete Binary Tree: A binary tree in which every level, except possibly the last, is completely filled, and all nodes are as far left as possible.
Full Binary Tree: A binary tree in which every node has either zero or two children.
Perfect Binary Tree: A binary tree in which all internal nodes have exactly two children, and all leaf nodes are at the same level.
Binary Search Tree (BST): A binary tree in which the value of each node in the left subtree is less than the value of the node itself, and the value of each node in the right subtree is greater than the value of the node itself.

```python
class TreeNode:
    def __init__(self, data):
        self.data = data
        self.children = []

    def add_child(self, child_node):
        self.children.append(child_node)

# Example usage:
if __name__ == "__main__":
    # Create nodes
    root = TreeNode("A")
    node_b = TreeNode("B")
    node_c = TreeNode("C")
    node_d = TreeNode("D")
    node_e = TreeNode("E")
    node_f = TreeNode("F")

    # Connect nodes
    root.add_child(node_b)
    root.add_child(node_c)
    node_b.add_child(node_d)
    node_b.add_child(node_e)
    node_c.add_child(node_f)

    # Print the tree structure
    def print_tree(node, level=0):
        print("  " * level + str(node.data))
        if node.children:
            for child in node.children:
                print_tree(child, level + 1)

    print_tree(root)
#Output
#A
#  B
#    D
#    E
#  C
#    F
```
Binary Tree Traversal
Going through a Tree by visiting every node, one node at a time, is called traversal.

Since Arrays and Linked Lists are linear data structures, there is only one obvious way to traverse these: start at the first element, or node, and continue to visit the next until you have visited them all.

But since a Tree can branch out in different directions (non-linear), there are different ways of traversing Trees.

There are two main categories of Tree traversal methods:

Breadth First Search (BFS) is when the nodes on the same level are visited before going to the next level in the tree. This means that the tree is explored in a more sideways direction.

Depth First Search (DFS) is when the traversal moves down the tree all the way to the leaf nodes, exploring the tree branch by branch in a downwards direction.

There are three different types of DFS traversals:

pre-order
```python
def preOrderTraversal(node):
    if node is None:
        return
    print(node.data, end=", ")
    preOrderTraversal(node.left)
    preOrderTraversal(node.right)
```
in-order
```python
def inOrderTraversal(node):
    if node is None:
        return
    inOrderTraversal(node.left)
    print(node.data, end=", ")
    inOrderTraversal(node.right)
```
post-order
```python
def postOrderTraversal(node):
    if node is None:
        return
    postOrderTraversal(node.left)
    postOrderTraversal(node.right)
    print(node.data, end=", ")
```
Binary Search tree:
A Binary Search Tree (BST) is a type of Binary Tree data structure, where the following properties must be true for any node "X" in the tree:

The X node's left child and all of its descendants (children, children's children, and so on) have lower values than X's value.
The right child, and all its descendants have higher values than X's value.
Left and right subtrees must also be Binary Search Trees.

Operations on Binary Search Trees:
Insertion: To insert a new node into a BST, you compare the value of the new node with the value of the current node. If it's less, you move to the left subtree; if it's greater, you move to the right subtree. This process continues until you find an appropriate empty spot to insert the new node.
Deletion: Deleting a node from a BST can be a bit more complex. There are several cases to consider:
If the node to be deleted has no children, you can simply remove it from the tree.
If the node has one child, you can replace the node with its child.
If the node has two children, you can either replace it with the minimum value node from its right subtree (or the maximum value node from its left subtree), or you can swap it with its successor (or predecessor) in the tree and then delete that successor node.
Search: To search for a value in a BST, you start at the root node and compare the target value with the current node's value. If they match, you've found the node. If the target value is less than the current node's value, you move to the left subtree; if it's greater, you move to the right subtree. This process continues recursively until you find the node with the target value or reach a leaf node.
Traversal: There are three primary ways to traverse a BST:
Inorder Traversal: Traverse the left subtree, visit the node, then traverse the right subtree. This results in a sorted list if the BST is balanced.
Preorder Traversal: Visit the node, then traverse the left and right subtrees.
Postorder Traversal: Traverse the left and right subtrees, then visit the node.
Complexity of Operations:
Search: The time complexity of searching in a BST is O(h), where h is the height of the tree. In a balanced BST, the height is logarithmic (O(log n)), where n is the number of nodes. However, in the worst-case scenario (when the tree is highly unbalanced), the height can be linear (O(n)), resulting in degraded performance.
Insertion and Deletion: Both operations require a search first, so their time complexity is also O(h). However, if rebalancing is necessary to maintain the BST property, additional operations may be required, resulting in a time complexity of O(log n) in balanced trees.


Benefits of Binary Search Trees:


Efficient Search: BSTs provide efficient searching due to their ordered structure, especially when the tree is balanced.
Dynamic Operations: BSTs allow dynamic insertion and deletion of nodes, making them suitable for applications with frequently changing data.
Simple Structure: BSTs have a simple and intuitive structure, making them easy to implement and understand.


Limitations of Binary Search Trees:


Degraded Performance: Unbalanced BSTs can lead to degraded performance, with search, insertion, and deletion operations taking linear time in the worst-case scenario.
Memory Consumption: The memory usage of a BST can grow significantly if the tree becomes unbalanced, potentially leading to inefficient use of memory resources.

AVL Tree:

An AVL tree is a self-balancing binary search tree named after its inventors, Adelson-Velsky and Landis. It maintains a strict balance criterion to ensure efficient insertion, deletion, and search operations with a guaranteed worst-case time complexity of O(log n), where n is the number of nodes in the tree. The balance criterion is based on the height difference (also known as the balance factor) between the left and right subtrees of any node.


Properties of AVL Trees:
Balance Factor: For any node in an AVL tree, the height of its left subtree and the height of its right subtree differ by at most 1.
Height: The height of an AVL tree is the maximum depth of any node in the tree. The height of an empty tree is considered -1.
Balanced Subtrees: In an AVL tree, all subtrees rooted at any node also satisfy the balance factor property.
Self-Balancing: After insertion or deletion of a node, AVL trees automatically perform rotations to maintain balance if necessary.


AVL Tree Rotations:
AVL trees use rotations to restore balance when it is violated due to insertion or deletion operations. There are four possible rotations:
Left Rotation: A rotation performed to restore balance when the right subtree is taller than the left subtree by more than one level.
Right Rotation: A rotation performed to restore balance when the left subtree is taller than the right subtree by more than one level.
Left-Right Rotation (LR Rotation): A combination of left rotation followed by right rotation used to balance the tree.
Right-Left Rotation (RL Rotation): A combination of right rotation followed by left rotation used to balance the tree.
Operations on AVL Trees:
Insertion: After inserting a new node, AVL trees check the balance factor of each node and perform rotations if necessary to restore balance.
Deletion: After deleting a node, AVL trees check the balance factor of each node and perform rotations if necessary to restore balance.
Search: Searching for a node with a given key in the AVL tree follows the same logic as in binary search trees with O(log n) time complexity.
Traversal: Inorder, preorder, and postorder traversal methods are applicable to AVL trees, providing access to all nodes in sorted order.
Height Calculation: AVL trees provide a height-balanced structure, ensuring that the height of the tree remains logarithmic.


Benefits of AVL Trees:
Efficiency: AVL trees offer efficient operations, ensuring O(log n) time complexity for insertion, deletion, and search operations.
Self-Balancing: AVL trees automatically adjust their structure to maintain balance, reducing the risk of performance degradation.
Predictability: The balance criterion of AVL trees ensures predictable performance characteristics, making them suitable for applications with strict performance requirements.


Limitations of AVL Trees:
Overhead: Maintaining balance in AVL trees requires additional overhead in terms of extra bookkeeping and rotations, impacting memory usage and performance.
Complexity: The implementation of AVL trees, especially rotation algorithms, can be more complex compared to simpler data structures like binary search trees.


### Hackerrank Challenge:
Q1. Consider a list (list = []). You can perform the following commands:

insert i e: Insert integer  at position .
print: Print the list.
remove e: Delete the first occurrence of integer .
append e: Insert integer  at the end of the list.
sort: Sort the list.
pop: Pop the last element from the list.
reverse: Reverse the list.
Initialize your list and read in the value of  followed by  lines of commands where each command will be of the  types listed above. Iterate through each command in order and perform the corresponding operation on your list.

```python
if __name__ == '__main__':
    N = int(input())
    lst = []

    for _ in range(N):
        command = input().split()

        if command[0] == 'insert':
            lst.insert(int(command[1]), int(command[2]))
        elif command[0] == 'print':
            print(lst)
        elif command[0] == 'remove':
            lst.remove(int(command[1]))
        elif command[0] == 'append':
            lst.append(int(command[1]))
        elif command[0] == 'sort':
            lst.sort()
        elif command[0] == 'pop':
            lst.pop()
        elif command[0] == 'reverse':
            lst.reverse()
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/47cf4689-f1e3-4ab6-9413-bb1a42b8ac53)

Q2. Given an integer, n, and  n space-separated integers as input, create a tuple,t , of those n integers. Then compute and print the result of hash(t).
```python
n = int(input())
integer_list = map(int, input().split())

t = tuple(integer_list)
result = hash(t)

print(result)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/cffab12e-ef0b-4928-a19a-fc6eeee8b7a5)

## Day 15 : Trees (contd.)

#### B-Tree:
Definition:

A B-tree is a self-balancing tree data structure designed to store and manage large amounts of data efficiently in secondary storage such as disks.
It was invented by Rudolf Bayer and Edward McCreight in 1972 as a generalization of binary search trees.
Properties:

In a B-tree, each node can contain a variable number of keys and pointers to child nodes.
The keys within a node are stored in sorted order, facilitating efficient search operations.
All leaf nodes are at the same level, which ensures balanced access to data across the entire tree.
B-trees are characterized by a parameter B, known as the "order" of the tree, which determines the maximum number of children a node can have.
A B-tree must satisfy certain properties, including the minimum degree requirement, which ensures that nodes have a minimum number of keys.
Operations:

Search: Similar to binary search trees, searching in a B-tree follows a recursive process, navigating through the tree based on the comparison of keys.
Insertion: Inserting a new key into a B-tree involves finding the appropriate position for the key and inserting it while maintaining the sorted order of keys within nodes.
Deletion: Deleting a key from a B-tree requires locating the key, removing it from the node, and potentially rebalancing the tree to maintain its properties.
Applications:

B-trees are widely used in databases and file systems for indexing and managing large datasets efficiently.
They are suitable for scenarios where data is stored on disk and must be accessed in blocks or pages.
#### B+ Tree:
Definition:

A B+ tree is a variation of the B-tree that enhances its structure for efficient range queries and sequential access.
It was introduced by Rudolf Bayer and Edward McCreight in 1972 and later popularized by Douglas Comer.
Properties:

Like a B-tree, a B+ tree consists of internal nodes and leaf nodes, with keys stored only in the leaf nodes.
All leaf nodes are linked together in a linked list, enabling efficient range queries and sequential access.
Internal nodes in a B+ tree act as index nodes, containing pointers to child nodes and dividing keys to guide searches.
Advantages:

B+ trees offer improved performance for range queries and sequential access due to the linked list structure of leaf nodes.
They are well-suited for database systems where range queries are common, such as retrieving all records within a specified range or performing range-based joins.
Operations:

The basic operations of insertion, deletion, and search in a B+ tree are similar to those in a B-tree.
Insertion and deletion may require additional operations to maintain the linked list structure of leaf nodes.
Applications:

B+ trees are widely used in database systems as indexing structures for efficient retrieval of data within a range.
They are also employed in file systems and operating systems for managing large files and directories efficiently.


General Tree (Inserting,Deleting,BFS and DFS):

```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.children = []

def insert_node(root, value):
    new_node = TreeNode(value)
    root.children.append(new_node)

def delete_node(root, value):
    for child in root.children:
        if child.value == value:
            root.children.remove(child)
            return
        delete_node(child, value)

def bfs(root):
    queue = [root]
    traversal = []
    while queue:
        node = queue.pop(0)
        traversal.append(node.value)
        for child in node.children:
            queue.append(child)
    return traversal

def dfs(root):
    traversal = []
    traversal.append(root.value)
    for child in root.children:
        traversal.extend(dfs(child))
    return traversal

# Example Usage
root = TreeNode(1)
insert_node(root, 2)
insert_node(root, 3)
insert_node(root.children[0], 4)
insert_node(root.children[0], 5)

print("BFS Traversal:", bfs(root))
print("DFS Traversal:", dfs(root))
```
Binary Tree :
```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

def insert_node(root, value):
    if root is None:
        return TreeNode(value)
    else:
        if value <= root.value:
            root.left = insert_node(root.left, value)
        else:
            root.right = insert_node(root.right, value)
    return root

def delete_node(root, value):
    if root is None:
        return root
    if value < root.value:
        root.left = delete_node(root.left, value)
    elif value > root.value:
        root.right = delete_node(root.right, value)
    else:
        if root.left is None:
            return root.right
        elif root.right is None:
            return root.left
        root.value = find_min_value(root.right)
        root.right = delete_node(root.right, root.value)
    return root

def find_min_value(root):
    min_value = root.value
    while root.left is not None:
        min_value = root.left.value
        root = root.left
    return min_value

def bfs(root):
    queue = [root]
    traversal = []
    while queue:
        node = queue.pop(0)
        traversal.append(node.value)
        if node.left:
            queue.append(node.left)
        if node.right:
            queue.append(node.right)
    return traversal

def dfs_inorder(root):
    if root is None:
        return []
    return dfs_inorder(root.left) + [root.value] + dfs_inorder(root.right)

# Example Usage
root = None
root = insert_node(root, 10)
root = insert_node(root, 5)
root = insert_node(root, 15)
root = insert_node(root, 3)
root = insert_node(root, 7)
root = insert_node(root, 12)
root = insert_node(root, 18)

print("BFS Traversal:", bfs(root))
print("DFS Inorder Traversal:", dfs_inorder(root))
```

Binary Search Tree:
```python
class TreeNode:
    def __init__(self, value):
        self.value = value
        self.left = None
        self.right = None

def insert_node(root, value):
    if root is None:
        return TreeNode(value)
    else:
        if value <= root.value:
            root.left = insert_node(root.left, value)
        else:
            root.right = insert_node(root.right, value)
    return root

def delete_node(root, value):
    if root is None:
        return root
    if value < root.value:
        root.left = delete_node(root.left, value)
    elif value > root.value:
        root.right = delete_node(root.right, value)
    else:
        if root.left is None:
            return root.right
        elif root.right is None:
            return root.left
        root.value = find_min_value(root.right)
        root.right = delete_node(root.right, root.value)
    return root

def find_min_value(root):
    min_value = root.value
    while root.left is not None:
        min_value = root.left.value
        root = root.left
    return min_value

def bfs(root):
    queue = [root]
    traversal = []
    while queue:
        node = queue.pop(0)
        traversal.append(node.value)
        if node.left:
            queue.append(node.left)
        if node.right:
            queue.append(node.right)
    return traversal

def dfs_inorder(root):
    if root is None:
        return []
    return dfs_inorder(root.left) + [root.value] + dfs_inorder(root.right)

# Example Usage
root = None
root = insert_node(root, 10)
root = insert_node(root, 5)
root = insert_node(root, 15)
root = insert_node(root, 3)
root = insert_node(root, 7)
root = insert_node(root, 12)
root = insert_node(root, 18)

print("BFS Traversal:", bfs(root))
print("DFS Inorder Traversal:", dfs_inorder(root))
```

### Top Questions related to Trees:
- Maximum Depth of Binary Tree
- Check if two trees have same structure
- Invert/Flip Binary Tree
- Binary Tree Maximum Path Sum
- Binary Tree Level Order Traversal
- Serialize and Deserialize Binary Tree
- Subtree of Another Tree
- Construct Binary Tree from Preorder and Inorder Traversal
- Validate Binary Search Tree
- Kth Smallest Element in a BST
- Lowest Common Ancestor of BST
- Implement Trie (Prefix Tree)
- Add and Search Word

### Hackerrank Challenge:
Q1. You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.
```python
def swap_case(s):
    swapped_string = ""
    for char in s:
        if char.isupper():
            swapped_string += char.lower()
        else:
            swapped_string += char.upper()
    return swapped_string

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
```
Output:

![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/1898685d-abaa-4a2a-83f5-0086b1de668e)

Q2. You are given a string. Split the string on a " " (space) delimiter and join using a - hyphen.

```python
def split_and_join(line):
    # Split the input string based on whitespace
    split_line = line.split()
    # Join the split parts using a hyphen as the delimiter
    joined_line = "-".join(split_line)
    return joined_line

if __name__ == '__main__':
    line = input()
    result = split_and_join(line)
    print(result)
```
Output:


![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/84d246e6-3950-4fb0-848d-47a01e839648)

## Day 16 : Array (Revision): 
TOP QUESTIONS IN ARRAY:
Q1. Find a peak element which is not smaller than its neighbours. Given an array arr of n elements that is first strictly increasing and then maybe strictly decreasing, find the maximum element in the array.

Note: If the array is increasing then just print the last element will be the maximum value.
```python
def findPeak(arr,n):
    #If an array has just one element
    if(n==1):
        return 0
    #If the array is in increasing order, just check the first element is greater or not
    if(arr[0]>=arr[1]):
        return 0
    #If the array is in decreasing order, just check the last element is greater or not
    if(arr[n-1]>=arr[n-2]):
        return n-1
    #for the rest of the elemnts if there is an increasing and decreasing combination in the array
    for i in range(1, n-1):
        if(arr[i]>=arr[i-1] and arr[i]>=arr[i+1]):
            return i
        
arr=[]
n=int(input("Enter the number of elements in the array: "))
for i in range(0, n):
    e=int(input("Enter element {}:".format(i+1)))
    arr.append(e)
print("Index of peak-point is: ",findPeak(arr,n)+1)
```
Output:
```
Enter the number of elements in the array: 6
Enter element 1:1
Enter element 2:3
Enter element 3:20
Enter element 4:4
Enter element 5:1
Enter element 6:0
Index of peak-point is:  3
```
Q2. Program to find the minimum (or maximum) element of an array Given an array, write functions to find the minimum and maximum elements in it.

```python
def minimum(arr,n):
    min_value = arr[0]
    for i in range (1, n):
        if(min_value>=arr[i]):
            min_value=arr[i]
    return min_value

def maximum(arr,n):
    max_value = arr[0]
    for i in range (1, n):
        if(max_value<=arr[i]):
            max_value=arr[i]
    return max_value

arr=[]
n=int(input("Enter the number of elements in the array: "))
for i in range(0, n):
    e=int(input("Enter element {}:".format(i+1)))
    arr.append(e)
print("Maximum Value:",maximum(arr,n))
print("Minimum Value:",minimum(arr,n))
```
Output:
```
Enter the number of elements in the array: 6
Enter element 1:5
Enter element 2:3
Enter element 3:7
Enter element 4:2
Enter element 5:6
Enter element 6:8
Maximum Value: 8
Minimum Value: 2
```
Q3. Given an array (or string), the task is to reverse the array/string.
```python
def reverse(arr, start, end):
    while(start<=end):
        arr[start], arr[end]= arr[end], arr[start]
        start+=1
        end-=1
    return arr

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("The reversed array : ",reverse(arr,0,n-1)) 
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 5
Enter element 2: 3
Enter element 3: 4
Enter element 4: 8
Enter element 5: 2
Enter element 6: 44
The reversed array :  [44, 2, 8, 4, 3, 5]
```
Q4. Write a program to sort a given array(in ascending order)
```python
def sort(arr,n):
    for i in range(0,n):
        min_e=i
        for j in range(i+1,n):
            if(arr[min_e]>arr[j]):
                min_e=j
        arr[min_e],arr[i]=arr[i],arr[min_e]
    return arr

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("The sorted array : ",sort(arr,n)) 
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 4
Enter element 2: 7
Enter element 3: 3
Enter element 4: 5
Enter element 5: 8
Enter element 6: 2
The sorted array :  [2, 3, 4, 5, 7, 8]
```
Q5. Find K-th smallest/largest element in the array
```python
def ksmall(arr,n):
    for i in range(0,n):
        min_e=i
        for j in range(i+1,n):
            if(arr[min_e]>arr[j]):
                min_e=j
        arr[min_e],arr[i]=arr[i],arr[min_e]
    return arr[k-1]

def klarge(arr,n):
    for i in range(0,n):
        min_e=i
        for j in range(i+1,n):
            if(arr[min_e]>arr[j]):
                min_e=j
        arr[min_e],arr[i]=arr[i],arr[min_e]
    return arr[n-k]

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
k=int(input("Enter the value of k: "))
print("The {}th smallest element :".format(k))
print(ksmall(arr,n))
print("The {}th largest element :".format(k))
print(klarge(arr,n))
Enter the number of elements in an array : 6
```
Output:
```
Enter element 1: 2
Enter element 2: 3
Enter element 3: 5
Enter element 4: 4
Enter element 5: 7
Enter element 6: 8
Enter the value of k: 2
The 2th smallest element :
3
The 2th largest element :
7
```
Q6. Count number of occurrences (or frequency) in a sorted array

Examples: Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 2 Output: 4 // x (or 2) occurs 4 times in arr[] Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 3 Output: 1 Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 1 Output: 2 Input: arr[] = {1, 1, 2, 2, 2, 2, 3,}, x = 4 Output: -1 // 4 doesn't occur in arr[]
```python
def occurence(arr,n,x):
    oc=0
    for i in range (0,n):
        if(arr[i]==x):
            oc+=1
    return oc

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
x=int(input("Enter the value of x for which the occurence is to be calculated: "))
print("Number of occurences : ",occurence(arr,n,x))
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: 3
Enter element 3: 3
Enter element 4: 4
Enter element 5: 4
Enter element 6: 4
Enter the value of x for which the occurence is to be calculated: 4
Number of occurences : 3
```
Q7. Given an array A[] consisting of only 0s, 1s, and 2s. The task is to write a function that sorts the given array. The functions should put all 0s first, then all 1s and all 2s in last.

This problem is also the same as the famous “Dutch National Flag problem”. The problem was proposed by Edsger Dijkstra. The problem is as follows:

Given N balls of colour red, white or blue arranged in a line in random order. You have to arrange all the balls such that the balls with the same colours are adjacent with the order of the balls, with the order of the colours being red, white and blue (i.e., all red coloured balls come first then the white coloured balls and then the blue coloured balls).
```python
def sort012(arr):
    l=0
    m=0
    h=n-1
    while(m<=h):
        #if arr[m] is equal to 0
        if(arr[m]==0):
            arr[l],arr[m]=arr[m],arr[l]
            l+=1
            m+=1
        #if arr[m] is equal to 1
        elif(arr[m]==1):
            m+=1
        #if arr[m] is equal to 2
        else:
            arr[m],arr[h]=arr[h],arr[m]
            h-=1
    return arr

n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("Sorted array : ",sort012(arr))
```
Output:
```
Enter the number of elements in an array : 6
Enter element 1: 0
Enter element 2: 1
Enter element 3: 2
Enter element 4: 0
Enter element 5: 1
Enter element 6: 2
Sorted array :  [0, 0, 1, 1, 2, 2]
```
### Hackerrank Challenge:
Q1. You are given the firstname and lastname of a person on two different lines. Your task is to read them and print the following:

Hello firstname lastname! You just delved into python.

```python
def print_full_name(first, last):
    # Print the message
    print("Hello", first, last + "!", "You just delved into python.")


if __name__ == '__main__':
    first_name = input()
    last_name = input()
    print_full_name(first_name, last_name)
```

Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/239ac5dc-b51c-4580-89ca-795c7bd54241)

Q2. We have seen that lists are mutable (they can be changed), and tuples are immutable (they cannot be changed).

Let's try to understand this with an example.

You are given an immutable string, and you want to make changes to it.

```python
def mutate_string(string, position, character):
    # Convert the string to a list to allow modifications
    string_list = list(string)
    
    # Replace the character at the specified position
    string_list[position] = character
    
    # Convert the list back to a string and return it
    return ''.join(string_list)

if __name__ == '__main__':
    s = input()
    i, c = input().split()
    s_new = mutate_string(s, int(i), c)
    print(s_new)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e17d3fdf-b75b-4d1f-acac-5838a04276d2)

## Day 17: Array Revision(contd.)
Q8. Given an array arr[] of non-negative integers and an integer sum, find a subarray that adds to a given sum. Note: There may be more than one subarray with sum as the given sum, print first such subarray.

Examples: Input: arr[] = {1, 4, 20, 3, 10, 5}, sum = 33 Output: Sum found between indexes 2 and 4 Explanation: Sum of elements between indices 2 and 4 is 20 + 3 + 10 = 33
```python
def subarray(arr,n,s):
    currentsum=arr[0]
    start=0
    i=1
    while(i<=n):
        while currentsum>s and start<=i-1:
            currentsum-=arr[start]
            start+=1
        if(currentsum==s):
            print("Sum found between indexes", start+1," and ",i)
            return 1
        if i<=n:
            currentsum+=arr[i]
        i+=1
    print("No subarray found")
    return 0
    
n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
s=int(input("Enter the value of sum : "))
subarray(arr,n,s)   
```
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: 2
Enter element 3: 3
Enter element 4: 4
Enter element 5: 5
Enter element 6: 9
Enter the value of sum : 7
Sum found between indexes 3  and  4
1
```
Q9. Move all negative numbers to beginning and positive to end with constant extra space
```python
def reArrange(arr, n): 
    low,high = 0, n - 1
    while(low<high): 
        if(arr[low] < 0): 
            low += 1
        elif(arr[high] > 0): 
            high -= 1
        else: 
            arr[low],arr[high] = arr[high],arr[low] 
  
def displayArray(arr, n): 
  
    for i in range(n): 
        print(arr[i],end = " ") 
    
    print('') 
    
    
n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
reArrange(arr,n)
displayArray(arr,n)
```
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: -1
Enter element 3: 2
Enter element 4: 4
Enter element 5: -3
Enter element 6: 5
-3 -1 2 4 1 5 
```
Q10. Given two sorted arrays, find their union and intersection.

Example:

Input: arr1[] = {1, 3, 4, 5, 7} arr2[] = {2, 3, 5, 6} Output: Union : {1, 2, 3, 4, 5, 6, 7} Intersection : {3, 5}

Input: arr1[] = {2, 5, 6} arr2[] = {4, 6, 8, 10} Output: Union : {2, 4, 5, 6, 8, 10} Intersection : {6}
```python
def find_union_and_intersection(arr1, arr2):
    m = len(arr1)
    n = len(arr2)
    union = []
    intersection = []
    i = 0
    j = 0

    while i < m and j < n:
        if arr1[i] == arr2[j]:
            intersection.append(arr1[i])
            union.append(arr1[i])
            i += 1
            j += 1
        elif arr1[i] < arr2[j]:
            union.append(arr1[i])
            i += 1
        else:
            union.append(arr2[j])
            j += 1

    # Add remaining elements of arr1 and arr2 to union
    while i < m:
        union.append(arr1[i])
        i += 1
    while j < n:
        union.append(arr2[j])
        j += 1

    return union, intersection

#Take user input for the arrays
arr1 = list(map(int, input("Enter the first sorted array elements separated by space: ").split()))
arr2 = list(map(int, input("Enter the second sorted array elements separated by space: ").split()))

#Call the function and print the results
union, intersection = find_union_and_intersection(arr1, arr2)
print("Union:", union)
print("Intersection:", intersection)
Enter the first sorted array elements separated by space: 1 2 3 4
Enter the second sorted array elements separated by space: 3 4 5
```
```
Union: [1, 2, 3, 4, 5]
Intersection: [3, 4]
```
Q11. Given an array, the task is to cyclically rotate the array clockwise by one time.

Examples:

Input: arr[] = {1, 2, 3, 4, 5} Output: arr[] = {5, 1, 2, 3, 4}

Input: arr[] = {2, 3, 4, 5, 1} Output: {1, 2, 3, 4, 5}
```python
def rotate(arr, n):
    last_el = arr[n - 1]
 
    for i in range(n - 1, 0, -1):
        arr[i] = arr[i - 1]
 
    arr[0] = last_el
 
 
n=int(input("Enter the number of elements in an array : "))
arr=[]
for i in range(0,n):
    e=int(input("Enter element {}: ".format(i+1)))
    arr.append(e)
print("Given array is :")
for i in range(0, n):
    print(arr[i], end=' ')
 
rotate(arr, n)
 
print("\nRotated array is :")
for i in range(0, n):
    print(arr[i], end=' ')
```
```
Enter the number of elements in an array : 6
Enter element 1: 1
Enter element 2: 4
Enter element 3: 5
Enter element 4: 2
Enter element 5: 3
Enter element 6: 8
Given array is :
1 4 5 2 3 8 
Rotated array is :
8 1 4 5 2 3 
```
### Hackerrank Challenge:
Q1. In this challenge, the user enters a string and a substring. You have to print the number of times that the substring occurs in the given string. String traversal will take place from left to right, not from right to left.

NOTE: String letters are case-sensitive.
```python
def count_substring(string, substring):
    count = 0
    sub_len = len(substring)
    for i in range(len(string) - sub_len + 1):
        if string[i:i+sub_len] == substring:
            count += 1
    return count


if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/b7059341-8917-40e3-be3a-90f0ae5a1edf)

Q2. You are given a string S .
Your task is to find out if the string S contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.

```python
def analyze_string(S):
    is_alphanumeric = False
    is_alphabetical = False
    is_digits = False
    is_lowercase = False
    is_uppercase = False

    for char in S:
        if char.isalnum():
            is_alphanumeric = True
        if char.isalpha():
            is_alphabetical = True
        if char.isdigit():
            is_digits = True
        if char.islower():
            is_lowercase = True
        if char.isupper():
            is_uppercase = True

    return is_alphanumeric, is_alphabetical, is_digits, is_lowercase, is_uppercase


if __name__ == '__main__':
    s = input()
    alphanumeric, alphabetical, digits, lowercase, uppercase = analyze_string(s)

    print(alphanumeric)
    print(alphabetical)
    print(digits)
    print(lowercase)
    print(uppercase)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a9cf7464-f534-4a8d-aaee-d81628be555e)

## Day 18: Trees (contd.)
Given a binary tree, the task is to find the height of the tree. The height of the tree is the number of vertices in the tree from the root to the deepest node.

```python
class Node:
 
    # Constructor to create a new node
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
 
# Compute the "maxDepth" of a tree -- the number of nodes
# along the longest path from the root node down to the
# farthest leaf node
 
 
def maxDepth(node):
    if node is None:
        return 0
 
    else:
 
        # Compute the depth of each subtree
        lDepth = maxDepth(node.left)
        rDepth = maxDepth(node.right)
 
        # Use the larger one
        if (lDepth > rDepth):
            return lDepth+1
        else:
            return rDepth+1
 
 
# Driver program to test above function
root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)
root.left.right = Node(5)
 
 
print("Height of tree is %d" % (maxDepth(root)))
```
Write a function to determine if two trees are identical or not:

Two trees are identical when they have the same data and the arrangement of data is also the same.
```python
class Node:
    # Constructor to create a new node
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
 
 
# Given two trees, return true if they are structurally
# identical
def identicalTrees(a, b):
 
    # 1. Both empty
    if a is None and b is None:
        return True
 
    # 2. Both non-empty -> Compare them
    if a is not None and b is not None:
        return ((a.data == b.data) and
                identicalTrees(a.left, b.left)and
                identicalTrees(a.right, b.right))
 
    # 3. one empty, one not -- false
    return False
 
 
# Driver code
root1 = Node(1)
root2 = Node(1)
root1.left = Node(2)
root1.right = Node(3)
root1.left.left = Node(4)
root1.left.right = Node(5)
 
root2.left = Node(2)
root2.right = Node(3)
root2.left.left = Node(4)
root2.left.right = Node(5)
 
# Function call
if __name__ == "__main__":
  if identicalTrees(root1, root2):
      print("Both trees are identical")
  else:
      print("Trees are not identical")
```
### Hackerrank Challenge
Q1. You are given a partial code that is used for generating the HackerRank Logo of variable thickness.
Your task is to replace the blank (______) with rjust, ljust or center.
```python
#Replace all ______ with rjust, ljust or center. 

thickness = int(input()) #This must be an odd number
c = 'H'

#Top Cone
for i in range(thickness):
    print((c*i).rjust(thickness-1)+c+(c*i).ljust(thickness-1))

#Top Pillars
for i in range(thickness+1):
    print((c*thickness).center(thickness*2)+(c*thickness).center(thickness*6))

#Middle Belt
for i in range((thickness+1)//2):
    print((c*thickness*5).center(thickness*6))    

#Bottom Pillars
for i in range(thickness+1):
    print((c*thickness).center(thickness*2)+(c*thickness).center(thickness*6))    

#Bottom Cone
for i in range(thickness):
    print(((c*(thickness-i-1)).rjust(thickness)+c+(c*(thickness-i-1)).ljust(thickness)).rjust(thickness*6))
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/31ae9d1c-19e3-473e-a57d-620d1a0589bc)
Q2. You are given a string S and width W.
Your task is to wrap the string into a paragraph of width w.
```python
import textwrap

def wrap(string, max_width):
    return textwrap.fill(string, max_width)

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a3365a17-bacf-4b1b-aceb-b1e4a225ea67)

## Day 19 : Trees (Problems contd.)
Given a binary tree, the task is to convert the binary tree into its Mirror tree. Mirror of a Binary Tree T is another Binary Tree M(T) with left and right children of all non-leaf nodes interchanged. 
```python
class newNode:
    def __init__(self, data):
        self.data = data
        self.left = self.right = None

def mirror(node):
 
    if (node == None):
        return
    else:
 
        temp = node
 
        """ do the subtrees """
        mirror(node.left)
        mirror(node.right)
 
        """ swap the pointers in this node """
        temp = node.left
        node.left = node.right
        node.right = temp
 
 
""" Helper function to print Inorder traversal."""
 
 
def inOrder(node):
 
    if (node == None):
        return
 
    inOrder(node.left)
    print(node.data, end=" ")
    inOrder(node.right)
 
 
# Driver code
if __name__ == "__main__":
 
    root = newNode(1)
    root.left = newNode(2)
    root.right = newNode(3)
    root.left.left = newNode(4)
    root.left.right = newNode(5)
 
    """ Print inorder traversal of
        the input tree """
    print("Inorder traversal of the",
          "constructed tree is")
    inOrder(root)
 
    """ Convert tree to its mirror """
    mirror(root)
 
    """ Print inorder traversal of 
        the mirror tree """
    print("\nInorder traversal of",
          "the mirror tree is ")
    inOrder(root)
```
### Hackerrank Challenge:
Q1. Mr. Vincent works in a door mat manufacturing company. One day, he designed a new door mat with the following specifications:

Mat size must be N*M. (N is an odd natural number, and M is 3 times N.)
The design should have 'WELCOME' written in the center.
The design pattern should only use |, . and - characters.
```python
def create_door_mat(N, M):
    # Top design
    for i in range(N // 2):
        pattern = '.|.' * (2 * i + 1)
        print(pattern.center(M, '-'))

    # Welcome message
    print('WELCOME'.center(M, '-'))

    # Bottom design (similar to top but reversed)
    for i in range(N // 2 - 1, -1, -1):
        pattern = '.|.' * (2 * i + 1)
        print(pattern.center(M, '-'))

N,M = map(int,input().split())
create_door_mat(N, M)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/bbe69871-046e-473b-8cc4-3a2492eaa9f0)

Q2.Given an integer,n , print the following values for each integer i from 1 to n:

Decimal
Octal
Hexadecimal (capitalized)
Binary
```python
def print_formatted(number):
    width = len("{0:b}".format(number))
    for i in range(1, number + 1):
        decimal = "{0:{width}d}".format(i, width=width)
        octal = "{0:{width}o}".format(i, width=width)
        hexadecimal = "{0:{width}X}".format(i, width=width)
        binary = "{0:{width}b}".format(i, width=width)
        print(decimal, octal, hexadecimal, binary)
if __name__ == '__main__':
    n = int(input())
    print_formatted(n)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/2bd54455-f8a6-4291-a246-9c1f14758fab)

## Day 21 : Trees (Problems contd.)
Diameter of Tree in O(n)
```python
class TreeNode:
    def __init__(self, val):
        self.val = val
        self.left = None
        self.right = None

def build_tree():
    val = input("Enter the value of the node (or type 'None' if it's a null node): ")
    if val.lower() == 'none':
        return None
    node = TreeNode(int(val))
    node.left = build_tree()
    node.right = build_tree()
    return node

def height_and_diameter(node):
    if not node:
        return 0, 0
    
    left_height, left_diameter = height_and_diameter(node.left)
    right_height, right_diameter = height_and_diameter(node.right)
    
    current_height = max(left_height, right_height) + 1
    current_diameter = max(left_height + right_height, left_diameter, right_diameter)
    
    return current_height, current_diameter

def diameter_of_binary_tree(root):
    _, diameter = height_and_diameter(root)
    return diameter
# Main function to build the binary tree and calculate its diameter
def main():
    print("Enter the nodes of the binary tree (enter 'None' for null nodes):")
    root = build_tree()
    print("Diameter of the binary tree:", diameter_of_binary_tree(root))

if __name__ == "__main__":
    main()
```
### Hackerrank Challenge:
Q1. You are given an integer, N. Your task is to print an alphabet rangoli of size N . (Rangoli is a form of Indian folk art based on creation of patterns.)
```python
def print_rangoli(size):
    import string
    
    # Create alphabet list
    alphabet = string.ascii_lowercase
    
    # Create the upper half of the rangoli
    for i in range(size-1, -size, -1):
        row = ['-'] * (2*size-1)
        for j in range(size - abs(i)):
            row[size - 1 - j] = alphabet[abs(i) + j]
            row[size - 1 + j] = alphabet[abs(i) + j]
        print('-'.join(row))

if __name__ == '__main__':
    n = int(input())
    print_rangoli(n)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/962a87e6-cab9-4508-b131-af199040f97d)

Q2.You are asked to ensure that the first and last names of people begin with a capital letter in their passports. For example, alison heck should be capitalised correctly as Alison Heck.
Given a full name, your task is to capitalize the name appropriately.
```python
#!/bin/python3

import math
import os
import random
import re
import sys

# Complete the solve function below.
def solve(s):
    return s.title()

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = solve(s)

    fptr.write(result + '\n')

    fptr.close()

```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/a5cdf9ae-19f1-4180-9def-1df77bd4b796)

## Day 22 : Trees (Problems contd.)
To check if a tree is height-balanced
```python
class Node:
    # Constructor to create a new Node
    def __init__(self, data):
        self.data = data
        self.left = None
        self.right = None
 
# function to find height of binary tree
 
 
def height(root):
 
    # base condition when binary tree is empty
    if root is None:
        return 0
    return max(height(root.left), height(root.right)) + 1
 
# function to check if tree is height-balanced or not
 
 
def isBalanced(root):
 
    # Base condition
    if root is None:
        return True
 
    # for left and right subtree height
    lh = height(root.left)
    rh = height(root.right)
 
    # allowed values for (lh - rh) are 1, -1, 0
    if (abs(lh - rh) <= 1) and isBalanced(
            root.left) is True and isBalanced(root.right) is True:
        return True
 
    # if we reach here means tree is not
    # height-balanced tree
    return False
 
 
# Driver function to test the above function
root = Node(1)
root.left = Node(2)
root.right = Node(3)
root.left.left = Node(4)
root.left.right = Node(5)
root.left.left.left = Node(8)
if isBalanced(root):
    print("Tree is balanced")
else:
    print("Tree is not balanced")
```
### Hackerrank Challenge:
Q1. You are asked to ensure that the first and last names of people begin with a capital letter in their passports. For example, alison heck should be capitalised correctly as Alison Heck.
Given a full name, your task is to capitalize the name appropriately.
```python
#!/bin/python3

import os

# Complete the solve function below.
def solve(s):
    return s.title()

if __name__ == '__main__':
    fptr = open(os.environ['OUTPUT_PATH'], 'w')

    s = input()

    result = solve(s)

    fptr.write(result + '\n')

    fptr.close()

```
Output:
![Screenshot 2024-02-15 212601](https://github.com/bijayaroy/python-daily-learning/assets/93483189/9c003fcf-2158-4f04-be08-54d0d29d607e)

Q2. User
Kevin and Stuart want to play the 'The Minion Game'.

Game Rules

Both players are given the same string,s .
Both players have to make substrings using the letters of the string s .
Stuart has to make words starting with consonants.
Kevin has to make words starting with vowels.
The game ends when both players have made all possible substrings.

Scoring
A player gets +1 point for each occurrence of the substring in the string s.

For Example:
String  = BANANA
Kevin's vowel beginning word = ANA
Here, ANA occurs twice in BANANA. Hence, Kevin will get 2 Points
```python
def minion_game(string):
    vowels = 'AEIOU'
    kevin_score = 0
    stuart_score = 0
    length = len(string)

    for i in range(length):
        if string[i] in vowels:
            kevin_score += length - i
        else:
            stuart_score += length - i

    if kevin_score > stuart_score:
        print("Kevin", kevin_score)
    elif kevin_score < stuart_score:
        print("Stuart", stuart_score)
    else:
        print("Draw")


if __name__ == '__main__':
    s = input()
    minion_game(s)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/d5db4d47-f284-4ac7-a1ab-89c40b464f1a)
## Day 23: 
### Hackerrank Challenge:
Q1. Consider the following:


A string, s, of length n where s = c0c1. . . . cn-1.

An integer, k, where k is a factor of n.

We can split s into n/k substrings where each subtring, ti, consists of a contiguous block of k characters in s. Then, use each ti to create string ui such that:

The characters in ui are a subsequence of the characters in ti.

Any repeat occurrence of a character is removed from the string such that each character in ui occurs exactly once. In other words, if the character at some index j in ti occurs at a previous index < j in ti, then do not include the character in string ui.

Given s and k, print n/k lines where each line i denotes string ui.

Example

s = “AAABCADDE”

k = 3

There are three substrings of length 3 to consider: ‘AAA’, ‘BCA’ and ‘DDE’. The first substring is all ‘A’ characters, so u1 = ‘A’. The second substring has all distinct characters, so u2 = ‘BCA’. The third substring has 2 different characters, so u3 = ‘DE’. Note that a subsequence maintains the original order of characters encountered. The order of characters in each subsequence shown is important.
```python
def merge_the_tools(string, k):
    temp = []
    len_temp = 0
    for item in string:
        len_temp += 1
        if item not in temp:
            temp.append(item)
        if len_temp == k:
            print (''.join(temp))
            temp = []
            len_temp = 0
if __name__ == '__main__':
    string, k = input(), int(input())
    merge_the_tools(string, k)
```
Output:
![image](https://github.com/bijayaroy/python-daily-learning/assets/93483189/e86c6c16-1ef9-4767-9b74-066b9ca60e2f)
