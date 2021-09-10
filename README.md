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

#### Mathematical Operations
Python
```python
first_value = 5
second_value = 4

sum = first_value + second_value
difference = first_value - second_value
product = first_value * second_value
quotient = first_value / second_value
modulus = first_value % second_value
exponent = first_value ** second_value 

print('Sum: ' + str(sum))
print('Difference: ' + str(difference))
print('Product: ' + str(product))
print('Quotient: ' + str(quotient))
print('Modulus: ' + str(modulus))
print('Exponent: ' + str(exponent))
```

Output
```output
Sum: 9
Difference: 1
Product: 20
Quotient: 1.25
Modulus: 1
Exponent: 625
```

#### Operators
```+```	Addition operator. <br>
```-```	Subtraction operator. <br>
```*```	Multiplication operator. <br>
```/```	Division operator. <br>
```%```	Modulus operator, which gives you the remainder (if any) after you divide one value into another. It's useful to know whether one value is evenly divisible by the other.. <br>
```**```Exponent operator. For example, "5 to the fourth power" is expressed as 5 * 5 * 5 * 5. <br>

#### Order of operations - PEDMAS
Parentheses: Resolve operations between parentheses first.<br>
Exponents: Resolve exponents.<br>
Multiplication: Perform multiplication, from left to right.<br>
Division: Perform division, from left to right.<br>
Addition: Perform addition, from left to right.<br>
Subtraction: Perform subtraction, from left to right.<br>

#### Mathematical Operations
Python
```python
print(3 + 4 * 5)
print((3 + 4) * 5)
```

Output
```output
23
35
```

#### Integers become floats
Python
```python
first_value = 5
second_value = 4

quotient = first_value / second_value

print(type(quotient))
print(quotient)
```

Output
```output
<class 'float'>
1.25
```

#### Floats become Integers
Python
```python
pi = 3.14
print(type(pi))
print(int(pi))

uptime = 99.99
print(type(uptime))
print(int(uptime))
```

Output
```output
<class 'float'>
3
<class 'float'>
99
```

#### Rounding numbers
Python
```python
pi = 3.14
print(type(pi))
print(int(pi))
print(round(pi))

uptime = 99.99
print(type(uptime))
print(int(uptime))
print(round(uptime))
```

Output
```output
<class 'float'>
3
3
<class 'float'>
99
100
```

#### Rounding numbers to a decimal place
Python
```python
first_value = round(7.654321, 2)
print(first_value)

second_value = round(9.87654, 3)
print(second_value)
```

Output
```output
7.65
9.877
```
