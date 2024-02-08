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
