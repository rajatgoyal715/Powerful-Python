
## Welcome to Python

Python is a programming language which can be used to make computer games, cross platform softwares, website applications and much more.


## Download and Installation

Visit the offical website - https://www.python.org/



## Math Basics


```python
# Addition

3 + 4
```




    7




```python
# Multiplication

5 * 20
```




    100




```python
# Bodmas

8 + 2 * 10
```




    28




```python
# Paranthesis

(8 + 2) * 10
```




    100




```python
# Float Division
# Returns the actual division output

18 / 4
```




    4.5




```python
# Integral Division
# Returns the integer part of the division

18 // 4
```




    4




```python
# Remainder

18 % 4
```




    2




```python
# Exponent

5 ** 3
```




    125



## Input/Output


```python
# Takes some input from the user
x = input('Input : ')

# Prints out the same as output
print('Output : ' + x)
```

    Input : 123abc!@#
    Output : 123abc!@#


## Data Types

### Integers


```python
x = 5
y = 5
```


```python
x + y
```




    10




```python
5 ** x
```




    3125



### Strings


```python
'String is comprised of characters in quotes'
```




    'String is comprised of characters in quotes'




```python
"It also works in double quotes"
```




    'It also works in double quotes'




```python
# 'I don't think if this works'
```


```python
# Escaping character

'I don\'t think this will create any problem.'
```




    "I don't think this will create any problem."




```python
# Use double quotes to remove this type of problem

"Just don't use single quotes!!"
```




    "Just don't use single quotes!!"




```python
# Formatting Characters

# Tab - '\t'
# Newline - '\n'

print('C:\Desktop\newfolder')
```

    C:\Desktop
    ewfolder



```python
# Use r to consider the raw string i.e. without any formatting

print(r'C:\Desktop\newfolder')
```

    C:\Desktop\newfolder



```python
# String multiplication

x = 'String '
x * 5
```




    'String String String String String '




```python
# String Concatenation

'Rajat ' + 'Goyal'
```




    'Rajat Goyal'




```python
# Integer to String Conversion

quantity = 5
denomination = " Rupees"

str(quantity) + denomination
```




    '5 Rupees'




```python
name = 'Rajat Goyal'

# Substring of a string by defining the range
name[3:8]
```




    'at Go'




```python
# Substring by defining the start index
name[6:]
```




    'Goyal'




```python
# Substring by defining the end index
name[:8]
```




    'Rajat Go'




```python
# Substring without any index specified will return the original string
name[:]
```




    'Rajat Goyal'




```python
# Print function which outputs the value on the console screen

print("Hello World")
```

    Hello World



```python
# Length of a string - Blankspace also counts as a character

len("Hello World")
```




    11



### Characters


```python
name = "Rajat Goyal"

# Access characters of string which is 0-indexed using square brackets
name[0]
```




    'R'




```python
# Access characters from the last using -1 indexing
name[-1]
```




    'l'



### Lists


```python
# Define a list of primitive data types

marks = [49, 53, 87, 65, 71]
```


```python
# Access the list which is 0-indexed i.e. (0, 1, 2, ... , n-1)

marks[0]
```




    49




```python
# Change any value in the list

marks[2] = 57

marks
```




    [49, 53, 57, 65, 71]




```python
# Add new elements to the list

updatedMarks = marks + [84, 68]
updatedMarks
```




    [49, 53, 57, 65, 71, 84, 68]




```python
# Add elements one at a time

marks.append(91)
marks
```




    [49, 53, 57, 65, 71, 91]




```python
# Sublist of a list

marks[:2]
```




    [49, 53]




```python
# Change sublist to a new list

marks[:2] = [0]
marks
```




    [0, 57, 65, 71, 91]



### Sets

Sets do not contain any element twice


```python
subjects = {'Mathematics', 'Physics', 'Chemistry', 'English', 'Economics'}
print(subjects)
```

    {'Chemistry', 'Mathematics', 'Physics', 'Economics', 'English'}



```python
if 'Physics' in subjects:
    print("It's gonna be fun!!")
else:
    print('-_-')
```

    It's gonna be fun!!


### Dictionaries

Dictionary is a set of key value pair


```python
students = {59:'Rajat', 64:'Rohan', 66:'Rohit'}

print(students)
print(students[64])
```

    {59: 'Rajat', 64: 'Rohan', 66: 'Rohit'}
    Rohan



```python
# Iterate over all elements of the dictionary

for key, value in students.items():
    print(str(key) + " : " + value)
```

    59 : Rajat
    64 : Rohan
    66 : Rohit


## Loops

### If


```python
age = 27

if age >= 18:
    print("I can vote now!")
```

    I can vote now!


### If-Else


```python
name = "Rajat"

if name is "Rajat":
    print('Hello Lord!')
else:
    print("I don't know ya")
```

    Hello Lord!


### If - Else If - Else


```python
num = 18

if num % 15 == 0:
    print("FooBar")
elif num % 5 == 0:
    print("Foo")
elif num % 3 == 0:
    print("Bar")
else:
    print("Nothing")
```

    Bar


### For


```python
foods = ['bacon', 'tuna', 'ham', 'beef']

for f in foods:
    print(f)
    print(len(f))
```

    bacon
    5
    tuna
    4
    ham
    3
    beef
    4


### Range


```python
# 1 argument - [0,n-1]
for x in range(5):
    print(x)
```

    0
    1
    2
    3
    4



```python
# 2 arguments - [a, b-1]
for x in range(1, 6):
    print(x)
```

    1
    2
    3
    4
    5



```python
# 3 arguments - arithmetic progression with 3rd argument as the difference
for x in range(0, 25, 5):
    print(x)
```

    0
    5
    10
    15
    20


### While


```python
num = 5

while num < 10:
    print("Num :", num)
    num += 1
```

    Num : 5
    Num : 6
    Num : 7
    Num : 8
    Num : 9


## Flow Control

### Break


```python
number = 5

for n in range(11):
    if n is number:
        print("Found the number!!")
        break
    print('-')
```

    -
    -
    -
    -
    -
    Found the number!!


### Continue


```python
number = 5

for n in range(11):
    if n is number:
        print("Skip the number!!")
        continue
    print(n)
```

    0
    1
    2
    3
    4
    Skip the number!!
    6
    7
    8
    9
    10


## Comments

### Single Line


```python
# This is a single line comment
```

### Multi Line


```python
print('Hello')

'''
Triple quotes are used for
    - multi
    - line
    - comments
'''

print('world')
```

    Hello
    world


## Functions


```python
# Defining a function
def sayHello():
    print('Hello World!')

# Calling the function
sayHello()
```

    Hello World!


### Parameters


```python
# Single Parameter

def feet_to_inches(feet):
    inches = 12 * feet
    print(str(feet) + " feet = " + str(inches) + " inches")

feet_to_inches(5)
feet_to_inches(6.2)
```

    5 feet = 60 inches
    6.2 feet = 74.4 inches



```python
# Multiple Parameters

def calculateSimpleInterest(amount, rate, time):
    interest = (amount * rate * time) / 100
    print(interest)
    
calculateSimpleInterest(1250, 5, 3)
```

    187.5


### Return Values


```python
# Return statement

def calculatePercentage(obtainedMarks, totalMarks):
    percentage = (obtainedMarks / totalMarks) * 100
    return percentage

print('I scored ' + str(calculatePercentage(323, 400)) + "%")
```

    I scored 80.75%


### Variable Scope


```python
a = 25 # Global variable

def funcA():
    b = 30 # Local variable
    print(a) # Prints out the global variable
    print(b) # Prints out the local variable
    
def funcB():
    print(a) # Prints out the global variable
    # print(b) # Variable b is not accessible here
    
funcA()
funcB()
```

    25
    30
    25


### Default Arguments


```python
# Default value for the parameter 'sex' is 'Unknown'
# This means that if no value is passed for the parameter 'sex', default value will be taken

def get_gender(sex='Unknown'):
    if sex is 'm':
        sex = 'Male'
    elif sex is 'f':
        sex = 'Female'
    print(sex)

get_gender('m')
get_gender('f')
get_gender()
```

    Male
    Female
    Unknown


### Keyword Arguments


```python
# Default value of 'time' is '1 year'
# With the help of keyword arguments, we can change specific arguments also

def calculateSimpleInterest(amount=1000, rate=2, time=1):
    interest = (amount * rate * time) / 100
    print(interest)
    
calculateSimpleInterest() # Default arguments
calculateSimpleInterest(1200, 5, 2)
calculateSimpleInterest(time=2) # Specific value for parameter 'time' only
calculateSimpleInterest(time=2, rate=5) # No need to maintain the correct order
```

    20.0
    120.0
    40.0
    100.0


### Flexible Number of Arguments


```python
# Use asterisk(*) to specify unknown number of arguments

def add_numbers(*args):
    total = 0
    for a in args:
        total += a
    print(total)
    
add_numbers()
add_numbers(3)
add_numbers(1, 2, 3, 4, 5)
```

    0
    3
    15


### Unpacking Arguments


```python
# Asterisk(*) does the unpacking of list into arguments

def calculateSimpleInterest(amount=1000, rate=2, time=1):
    interest = (amount * rate * time) / 100
    print(interest)

data = [1200, 5, 2]

calculateSimpleInterest(data[0], data[1], data[2])
calculateSimpleInterest(*data)
```

    120.0
    120.0


## Modules

With the help of modules, there is no need to rewrite functions over and over again.


```python
# Create a file test.py which acts as a module

# Import the module(thus importing all functions in it)
import test

# Call the function using the module name
test.hello()
```

    Hello World



```python
import random

x = random.randrange(1, 1000)
print(x)
```

    220



```python
# From 'test' module, import specific function 'hello'
from test import hello

hello()
```

    Hello World


### Download an image from the web


```python
import urllib.request

def download_web_image(url):
    urllib.request.urlretrieve(url, 'images/image.png')
    
download_web_image("https://www.python.org/static/opengraph-icon-200x200.png")
```

### Read and write files


```python
fw = open('sample.txt', 'w')

for i in range(5):
    fw.write(str(i) + '\n')

fw.close()
```


```python
fr = open('sample.txt', 'r')

data = fr.read()
print(data)

fr.close()
```

    0
    1
    2
    3
    4
    


## Exception


```python
while True:
    try:
        x = int(input('\nEnter a number \n'))
        print(50/x)
        break
    except ValueError:
        # If input contains anything other than digits
        print('Oops! Please enter a number only.')
    except ZeroDivisionError:
        # If input is equal to zero
        print("Don't pick zero")
    except:
        # All other errors will be caught by this method
        break
    finally:
        # This is called in every case
        print('Loop complete')
```

    
    Enter a number 
    abc
    Oops! Please enter a number only.
    Loop complete
    
    Enter a number 
    0
    Don't pick zero
    Loop complete
    
    Enter a number 
    123
    0.4065040650406504
    Loop complete


## Classes and Objects


```python
class Class:
    
    variable = 10
    
    def incrementVariable(self):
        self.variable += 1
        
    def decrementVariable(self):
        self.variable -= 1
        
    def printVariable(self):
        print(self.variable)
```


```python
# Creating an object
obj = Class()

# Calling the member functions of the class using the object
obj.printVariable()
obj.incrementVariable()
obj.printVariable()
obj.decrementVariable()
obj.printVariable()
```

    10
    11
    10



```python
# Different objects have different memory blocks associated for class member variables
obj1 = Class()
obj2 = Class()

obj1.incrementVariable()
obj2.decrementVariable()

obj1.printVariable()
obj2.printVariable()
```

    11
    9


### init function


```python
class Class:
    
    # Constructor helps in constructing objects
    def __init__(self, x=10):
        self.variable = x
        
    def printVariable(self):
        print(self.variable)
```


```python
# Initiating an object will first call the constructor i.e init function
obj = Class()
obj1 = Class(32)

obj.printVariable()
obj1.printVariable()
```

    10
    32


### Class Variables vs Instance Variables


```python
class Girl:
    
    # Class variables are shared by all instances of the class
    gender = 'female'
    
    def __init__(self, name):
        # For each object of the class, instance variables are different
        self.name = name
        
r = Girl('name1')
s = Girl('name2')

print(r.gender)
print(s.gender)
print(r.name)
print(s.name)
```

    female
    female
    name1
    name2


## Inheritance


```python
class Parent():
    
    def print_last_name(self):
        print('Last Name')


class Child(Parent):
    
    def print_first_name(self):
        print('First Name')


child = Child()
child.print_first_name()

# We can call the parent class functions also on any object of child class
child.print_last_name()
```

    First Name
    Last Name


### Overriding


```python
class Parent():
    
    def print_last_name(self):
        print('Last Name')
        

class Child(Parent):
    
    def print_first_name(self):
        print('First Name')
    
    # Overriding a function already present in the parent class
    def print_last_name(self):
        print('Another Last Name')
        
        
child = Child()
child.print_first_name()

# New function defined in child class overrides the parent function
child.print_last_name()
```

    First Name
    Another Last Name


## Multiple Inheritance

Inherting the functions from two or more classes


```python
class A():
    
    def funcA(self):
        print('Function of class A')
    
class B():

    def funcB(self):
        print('Function of class B')

# Multiple inheritance
class C(A, B):
    
    # If no function or class variable in present in class, we have to write the keyword 'pass'
    pass

c = C()
c.funcA()
c.funcB()
```

    Function of class A
    Function of class B


## Threading


```python
import threading

class Messenger(threading.Thread):
    
    def run(self):
        for _ in range(10):
            print(threading.currentThread().getName())
            
x = Messenger(name = 'Send out messages')
y = Messenger(name = 'Receive messages')

x.start()
y.start()
```

    Send out messagesReceive messages
    
    Receive messages
    Send out messagesReceive messages
    


### Unpacking Lists


```python
details = ['Rajat', 'Goyal', 20]

# Unpacking a list into different variables
first_name, last_name, age = details

print(first_name)
print(last_name)
print(age)
```

    Send out messagesReceive messages
    
    Send out messagesReceive messages
    
    Receive messagesSend out messages
    
    Receive messagesSend out messages
    
    Receive messagesSend out messages
    
    Receive messagesSend out messages
    
    Receive messagesSend out messages
    
    Send out messages
    Rajat
    Goyal
    20



```python
# In the above example, we knew the number of elements(attributes) present in the list
# We can use asterisk(*) to store the remaining elements of the list

marks = [23, 26, 76, 45, 59, 38, 94, 43]

first, *remaining, last = marks

print(first)
print(remaining)
print(last)
```

    23
    [26, 76, 45, 59, 38, 94]
    43


### Zip function

Attach two lists together


```python
first = ['Bruce', 'Tom', 'Taylor']
last = ['Wayne', 'Hanks', 'Swift']

names = zip(first, last)

for a, b in names:
    print(a, b)
```

    Bruce Wayne
    Tom Hanks
    Taylor Swift


### Lambda function

function_name = lambda parameter: computation


```python
answer = lambda x: x*5
print(answer(5))
```

    25


### Min, Max and Sorting Dictionaries


```python
marks = {
    'physics' : 93,
    'mathematics' : 95,
    'chemistry' : 93,
    'english' : 90,
    'physical education' : 98
}

# Minimum according to the alphabetical order of keys
print(min(zip(marks.keys(), marks.values())))

# Minimum according to the numerical value
print(min(zip(marks.values(), marks.keys())))

# Maximum of all the values
print(max(zip(marks.values(), marks.keys())))

# Sorted list of tuples
print(sorted(zip(marks.values(), marks.keys())))
```

    ('chemistry', 93)
    (90, 'english')
    (98, 'physical education')
    [(90, 'english'), (93, 'chemistry'), (93, 'physics'), (95, 'mathematics'), (98, 'physical education')]


### Struct


```python
from struct import *

# Store as bytes data
packed_data = pack('iif', 6, 19, 4.73)
print(packed_data)
```

    b'\x06\x00\x00\x00\x13\x00\x00\x00)\\\x97@'



```python
print(unpack('iif', packed_data))
```

    (6, 19, 4.730000019073486)


### Map function


```python
income = [10, 30, 75]

def double_money(money):
    return money * 2

new_income = list(map(double_money, income))
print(new_income)
```

    [20, 60, 150]


## Bitwise Operators

### AND


```python
a = 50     # 110010
b = 25     # 011001

c = a & b  # 010000
print(c)
```

    16


### OR


```python
a = 50     # 110010
b = 25     # 011001

c = a | b  # 111011
print(c)
```

    59


### Left and Right Shift


```python
a = 240     # 11110000

# Left shift
b = a << 2  # 1111000000
print(b)

# Right shift
b = a >> 2  # 00111100
print(b)
```

    960
    60


### Finding Largest or Smallest Items


```python
import heapq

grades = [32, 43, 654, 34, 132, 66, 99, 532]

print(heapq.nlargest(3, grades))
```

    [654, 532, 132]



```python
stocks = [
    {'ticker': 'AAPL', 'price': 201},
    {'ticker': 'GOOG', 'price': 800},
    {'ticker': 'F', 'price': 54},
    {'ticker': 'MSFT', 'price': 313},
    {'ticker': 'YHOO', 'price': 68},
]

print(heapq.nsmallest(2, stocks, key=lambda stock: stock['price']))
```

    [{'ticker': 'F', 'price': 54}, {'ticker': 'YHOO', 'price': 68}]


### Finding most frequent items


```python
from collections import Counter

text = "Python can be easy to pick up whether you're a first time programmer or you're experienced with other languages. The following pages are a useful first step to get on your way writing programs with Python!"

words = text.split()

counter = Counter(words)
top_three = counter.most_common(3)
print(top_three)
```

    [('to', 2), ("you're", 2), ('a', 2)]

