# Python Basics: For References

# Table of Contents
1. [Variables](https://github.com/Athena-Gerardo/PythonPortfolio/blob/main/README.md#variables)
2. [Data Types](https://github.com/Athena-Gerardo/PythonPortfolio/blob/main/README.md#data-types)

## Variables

Python will reference the most recent assignment for a variable, unless the variables are different cases (python is case-sensitive)
```python
x = 4
x = "Sally"
print(x)
```
Legal variable names in Python:
```python
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```
Many values to multiple variables, or one value to multiple variables
```python
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)

x = y = z = "Orange"
print(x)
print(y)
print(z)
```
Collections
```python
fruits = ["kiwi", "plum", "apple"] 
x, y, z = fruits #this will assign the variables to the collection accordingly
print(x)
print(y)
print(z)
```
Output variables
You can use , or + to print variables, however, + is used for addition with number variables and combining numbers with non numbers using + will result in an error
```python
x = "Python"
y = "is"
z = "awesome"
print(x, y, z) #OR print(x + y + z) but you need to put a space after each word, or else it will print "Pythonisawsome"
```
Global Variables: variables created outside of a function, and can be used inside and outside of functions
```python
x = "cool" #This is a global variable

def myfunc():
  print("Python is " + x)

myfunc()
```
If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.
```python
x = "cool"

def myfunc():
  x = "awesome" #this is a local variable
  print("Python is " + x)

myfunc() #this will result with the local variable, unless you use global in the function, then that will create a global variable within the function and replace any global variables already called to

print("Python is " + x) #this will result with the global variable
```

## Data Types

Python has the following data types built-in by default, in these categories:
* Text Type:	str
* Numeric Types:	int, float, complex
* Sequence Types:	list, tuple, range
* Mapping Type:	dict
* Set Types:	set, frozenset
* Boolean Type:	bool
* Binary Types:	bytes, bytearray, memoryview
* None Type:	NoneType
** Note: use print(type()) to find out the variable's data type

Python will automatically assign a data type when a variable is declared:
* x = "Hello World":	str	
* x = 20:	int	
* x = 20.5:	float	
* x = 1j:	complex	
* x = ["apple", "banana", "cherry"]:	list	
* x = ("apple", "banana", "cherry"):	tuple	
* x = range(6):	range	
* x = {"name" : "John", "age" : 36}:	dict	
* x = {"apple", "banana", "cherry"}:	set	
* x = frozenset({"apple", "banana", "cherry"}):	frozenset	
* x = True:	bool	
* x = b"Hello":	bytes	
* x = bytearray(5):	bytearray	
* x = memoryview(bytes(5)):	memoryview	
* x = None:	NoneType

Casting: can use multiple types, and recall the type using type(). When casting, or setting the specific data type, use the abbreviation associated with that data type. (Refer to the list above for all abbreviations.)
```python
x = str(3) # x will be '3'
y = int(3) # y will be 3
z = float(3) #z will be 3.0
print(type(x))
```


## Strings

Slicing, index starts at 0, does not include last number of index (if specified):
```python
b = "Hello, World!"
print(b[2:5]) # or print(b[2:]) or print(b[:5])
```

Modify, with upper, lower, or strip:
```python
a = "Hello, World!"
print(a.upper())
print(a.lower())
print(a.strip()) # removes whitespace (space before and/or after the acutal text)
```

Concatenate:
```python
a = "Hello"
b = "World"
c = a + b # add "+ " " +" if a space is needed inbetween words
print(c)
```

Format/F-Strings, used to combine str and num into one:
```python
age = 36
txt = f"My name is John, I am {age}"
print(txt)
```
Placeholders, can contain variables, operations, functions, and modifiers to format the value:
```python
txt = f"The price is {20 * 59} dollars"
print(txt)
```
Modifiers, use ":" after the variable's name within the placeholder:
```python
price = 59
txt = f"The price is {price:.2f} dollars" # .2f is the fixed decimal place that is desired to display
print(txt)
```

Escape
```python

```

Methods:
```python

```
