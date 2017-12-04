
## Welcome to Python

Python is a programming language which can be used to make computer games, cross platform softwares, website applications and much more.


## Download and Installation

Visit the offical website - https://www.python.org/


## Introduction

This notebook is made from the python tutorial series by Bucky.
This notebook is developed using Python 3.


## Editors

You can use IDLE, Sublime, Atom, Visual Studio Code or any other editor.


## Basics


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
# Power

5 ** 3
```




    125



## Variables

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
'I don't think if this works'
```


      File "<ipython-input-14-f8997715f0be>", line 1
        'I don't think if this works'
               ^
    SyntaxError: invalid syntax




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
def sayHello():
    print('Hello World!')
    
sayHello()
```

    Hello World!

