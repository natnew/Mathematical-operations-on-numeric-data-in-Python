# Mathematical-operations-on-numeric-data-in-Python 🐍
Mathematical operations on numeric data in Python
More information can be found here: https://docs.microsoft.com/en-us/learn/modules/python-datatypes-numeric-operations/
There are many situations where you may receive string data that you need to convert into a integer or you need to perform calculations on numeric data. Python provides in-built features for mathematical manipulation. This repo consist of small python mathematical exercises.

## Task 1

#### Find the type of a value
Python
```python
print(type('7'))
print(type(7))
print(type(7.1))
```

Output
```output
<class 'str'>
<class 'int'>  
<class 'float'>
```

#### Find the type of a value using isinstance()
Python
```python
print(isinstance('7', str))
print(isinstance(7, int))
print(isinstance(7.1, float))

print(isinstance(7, str))
print(isinstance('7', int))
print(isinstance('7.1', float))
```

Output
```output
True
True 
True 
False
False
False
```

#### Create a boolean using isinstance()
Python
```python
print(type('7') == str)
print(type(7) == int)
print(type(7.1) == float)

print(type(7) == str)
print(type('7') == int)
print(type('7.1') == float)
```

Output
```output
True
True 
True 
False
False
False
```

#### Find the relationship between data types
Python
```python
x = 'a string'
print(type(x))
x = 7
print(type(x))
x = False 
print(type(x))
```

Output
```output
<class 'str'>
<class 'int'>
<class 'bool'>
```

## Task 2
```isalnum()```	Ensures that the string has no special characters, such as %, $, #, @, or !. <br>
```isalpha()```	Ensures that the string contains only letters of the alphabet. <br>
```isdecimal()```	Ensures that the string contains only decimal values (numbers). <br>
```istitle()```	Ensures that the string follows the rules of capitalization (as in a sentence). <br>
```isupper()```	Ensures that the string contains only uppercase letters. <br>
```islower()```	Ensures that the string contains only lowercase letters.<br>

#### Use IF statement with isnumeric()
Python
```python
first_value = input('First Number: ')

if first_value.isnumeric() == False:
    print('Value is not a number.')
    exit()

second_value = input('Second Number: ')

if second_value.isnumeric() == False:
    print('Value is not a number.')
    exit()

first_value = int(first_value)
second_value = int(second_value)

sum = first_value + second_value
print('Sum: ' + str(sum))
```

Output
```output
First Number: 4
Second Number: 5
Sum: 9
```

#### Use IF/OR statement with isnumeric()
Python
```python
first_value = input('First Number: ')
second_value = input('Second Number: ')

if first_value.isnumeric() == False or second_value.isnumeric() == False:
    print('Please enter numbers only.')
    exit()

first_value = int(first_value)
second_value = int(second_value)

sum = first_value + second_value
print('Sum: ' + str(sum))
```

Output
```output
First Number: 4
Second Number: 5
Sum: 9
```

## Task 3
