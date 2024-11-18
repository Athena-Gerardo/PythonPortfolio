/*

Python Basics

For references

*/

# Table of Contents


## Variables

# Python will reference the most recent assignment for a variable, unless the variables are different cases (python is case-sensitive)
```python
x = 4
x = "Sally"
print(x)
```
# Casting: can use multiple types, and recall the type using type()
x = str(3) # x will be '3'
y = int(3) # y will be 3
z = float(3) #z will be 3.0
print(type(x))

# Legal variable names in Python:
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"

# Many values to multiple variables, or one value to multiple variables
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)

x = y = z = "Orange"
print(x)
print(y)
print(z)

# Collections
fruits = ["kiwi", "plum", "apple"] 
x, y, z = fruits #this will assign the variables to the collection accordingly
print(x)
print(y)
print(z)

# Output variables
# You can use , or + to print variables, however, + is used for addition with number variables and combining numbers with non numbers using + will result in an error
x = "Python"
y = "is"
z = "awesome"
print(x, y, z) #OR print(x + y + z) but you need to put a space after each word, or else it will print "Pythonisawsome"

# Global Variables: variables created outside of a function, and can be used inside and outside of functions
x = "cool" #This is a global variable

def myfunc():
  print("Python is " + x)

myfunc()

# If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.
x = "cool"

def myfunc():
  x = "awesome" #this is a local variable
  print("Python is " + x)

myfunc() #this will result with the local variable, unless you use global in the function, then that will create a global variable within the function and replace any global variables already called to

print("Python is " + x) #this will result with the global variable


## Data Types
