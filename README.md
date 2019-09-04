# Python-Tutorial

## Python Course Outline



1. Getting Started
    1. About this course
    2. Why Python
    3. Installation
2. Basic Syntax
    4. Hello World
    5. Lines & Indentation
    6. Python Identifiers
    7. Reserved Words
    8. User inputs
    9. Comments in python
    10. Quotation in python
    11. Multi-line statements
3. Variable Types
    12. Assigning values to variables
    13. Multiple line Assigiments
    14. Standard data types - numbers, lists, strings, dictionary, tuple
4. Basic Operators
5. Decision Making
6. Loops
7. Numbers
8. Strings
9. Lists 
10. Tuples
11. Dictionary
12. Functions
13. Advanced Topics

Resources:


1. [https://docs.python.org/3/tutorial/appetite.html](https://docs.python.org/3/tutorial/appetite.html)
2. [https://github.com/vivianakinyi/python101/](https://github.com/vivianakinyi/python101/)
3. [https://www.tutorialspoint.com/python/index.htm](https://www.tutorialspoint.com/python/index.htm)
4. [https://www.codecademy.com/learn/learn-python](https://www.codecademy.com/learn/learn-python)
5. [https://www.python-course.eu/](https://www.python-course.eu/)
6. [https://www.learnpython.org/](https://www.learnpython.org/)
7. [https://www.geeksforgeeks.org/python-programming-language/](https://www.geeksforgeeks.org/python-programming-language/)



1. Getting Started
    1. About this course

This course aims to teach the basics of programming computers using Python. We cover the basics of how one constructs a program from a series of simple instructions in Python.  The course has no pre-requisites and avoids all but the simplest mathematics. Anyone with moderate computer experience should be able to master the materials in this course. There are two major Python versions, Python 2 and Python 3. Python 2 and 3 are quite different. This course covers Python 2, but we will mention the differences as we go on.



    2. Why Learn Python

Python is a general-purpose, versatile and popular programming language. It’s great as a first language because it is concise and easy to read, and it is also a good language to have in any programmer’s stack as it can be used for everything from web development to software development and scientific applications such as data mining and machine learning.

Fun Fact: Python is named after the BBC show “Monty Python’s Flying Circus” and has nothing to do with reptiles.



    3. Installation

    Python is available on a wide variety of platforms including Windows, Linux and Mac OS X. 


Getting Python


    The most up-to-date and current source code, binaries, documentation, news, etc., is available on the official website of Python [https://www.python.org/](https://www.python.org/)


    You can download Python documentation from [https://www.python.org/doc/](https://www.python.org/doc/). 


### 
    Windows Installation


    Here are the steps to install Python on Windows machine.



*   Open a Web browser and go to [https://www.python.org/downloads/](https://www.python.org/downloads/).
*   Follow the link for the Windows installer _python-2.7.msi_ file 
*   To use this installer _python-2.7.msi_, the Windows system must support Microsoft Installer 2.0. Save the installer file to your local machine and then run it to find out if your machine supports MSI.
*   Run the downloaded file. This brings up the Python install wizard, which is really easy to use. Just accept the default settings, wait until the install is finished, and you are done.


### Unix and Linux Installation


    Python comes pre-installed on all versions after Ubuntu 14.04. you can access it by typing the following into the terminal for Python 2


    $ python


    If you don’t have Python 2 installed then, you can install it by typing the following into the terminal :



1. `sudo add-apt-repository ppa:fkrull/deadsnakes-python2.7`
2. <code>sudo apt-<strong>get</strong> update</code>
3. <code>sudo apt-<strong>get</strong> install python2.7</code>

    Alternatively


    Here are the simple steps to install Python on Unix/Linux machine.

*   Open a Web browser and go to [https://www.python.org/downloads/](https://www.python.org/downloads/).
*   Follow the link to download zipped source code available for Unix/Linux.
*   Download and extract files.
*   Editing the _Modules/Setup_ file if you want to customize some options.
*   run ./configure script
*   make
*   make install

    This installs Python at standard location _/usr/local/bin_ and its libraries at _/usr/local/lib/pythonXX_where XX is the version of Python.



### Macintosh Installation


    Recent Macs come with Python installed, but it may be several years out of date. See [http://www.python.org/download/mac/](https://www.python.org/download/mac/) for instructions on getting the current version along with extra tools to support development on the Mac. For older Mac OS's before Mac OS X 10.3 (released in 2003), MacPython is available.


## Setting up PATH


    Programs and other executable files can be in many directories, so operating systems provide a search path that lists the directories that the OS searches for executables.


    The path is stored in an environment variable, which is a named string maintained by the operating system. This variable contains information available to the command shell and other programs.


    The path variable is named as PATH in Unix or Path in Windows (Unix is case sensitive; Windows is not).


    In Mac OS, the installer handles the path details. To invoke the Python interpreter from any particular directory, you must add the Python directory to your path.


## Setting path at Unix/Linux


    To add the Python directory to the path for a particular session in Unix −



*   In the csh shell − type setenv PATH "$PATH:/usr/local/bin/python" and press Enter.
*   In the bash shell (Linux) − type export PATH="$PATH:/usr/local/bin/python" and press Enter.
*   In the sh or ksh shell − type PATH="$PATH:/usr/local/bin/python" and press Enter.
*   Note − /usr/local/bin/python is the path of the Python directory


## Setting path at Windows


    To add the Python directory to the path for a particular session in Windows −


    At the command prompt − type path %path%;C:\Python and press Enter.


    Note − C:\Python is the path of the Python directory


## Running Python


    There are three different ways to start Python −


### Interactive Interpreter


    You can start Python from Unix, DOS, or any other system that provides you a command-line interpreter or shell window.


    Enter python the command line.


    Start coding right away in the interactive interpreter.


```
$python # Unix/Linux
or
python% # Unix/Linux
or
C:> python # Windows/DOS
```



### Script from the Command-line


    A Python script can be executed at command line by invoking the interpreter on your application, as in the following −


```
$python script.py # Unix/Linux
or
python% script.py # Unix/Linux
or 
C: >python script.py # Windows/DOS
```



    Note − Be sure the file permission mode allows execution.


### Integrated Development Environment


    You can run Python from a Graphical User Interface (GUI) environment as well, if you have a GUI application on your system that supports Python.



*   Unix − IDLE is the very first Unix IDE for Python.
*   Windows − PythonWin is the first Windows interface for Python and is an IDE with a GUI.
*   Macintosh − The Macintosh version of Python along with the IDLE IDE is available from the main website, downloadable as either MacBinary or BinHex'd files.
2. **Basic Syntax**
    4. Hello World - Our First Python Program

Let us now create our very first python program. We will show you two ways to print “Hello World” in python.

**Using the python Interpreter**

With the Python interactive interpreter it is easy to check Python commands. The Python interpreter can be invoked by typing the command "python" without any parameter followed by the "return" key at the shell prompt:

In your terminal/shell type

$python

This should open up an interactive prompt as shown below

Python 2.7.15+ (default, Nov 27 2018, 23:36:35) 

[GCC 7.3.0] on linux2

Type "help", "copyright", "credits" or "license" for more information.

>>>

Type the following text at the Python prompt “>>>”” and press the Enter −

>>> print “Hello, World!”

Note: To close the Python interactive interpreter in Linux type Ctrl-D

**Execute a Python Script**

Now we will create a python program using a script file. Python scripts have a .py extension.

To save and edit programs in a file we need an editor. There are lots of editors, but you should choose one, which supports syntax highlighting and indentation. Under Linux you can use vi, vim, emacs, geany, gedit and umpteen others including sublime, pycharm notebook++ etc

Create a file and name it as hello.py

Type the following in the hello.py file and save it

print “Hello, World!”

We assume that you have Python interpreter set in PATH variable. Now, try to run this program as follows −

$ python hello.py

The result should be:

Hello, World!

Congratulations, you just created your very first python program!



    5. **Lines & Indentation**

Python uses indentation for blocks, instead of curly braces. Both tabs and spaces are supported, but the standard indentation requires standard Python code to use four spaces.

The number of spaces in the indentation is variable, but all statements within the block must be indented the same amount. For Example

<insert example>



    6. **Reserved Words**
    7. **Quotation in python**

    Python accepts single ('), double (") and triple (''' or """) quotes to denote string literals, as long as the same type of quote starts and ends the string.

    8. **Multi-line statements**

Statements in Python typically end with a new line. Python does, however, allow the use of the line continuation character (\) to denote that the line should continue. For example −



    9. **Comments in python**

A hash sign (#) that is not inside a string literal begins a comment. All characters after the # and up to the end of the physical line are part of the comment and the Python interpreter ignores them.

Tripled quoted strings are also comments  and mainly used for mutti-line comments. For Example:



3. **User inputs**

In python a user can be prompt to enter a value or take an action using the following:

input(“Enter a yes or no”)



4. **Data Types and Variables**

    **Variables**


    A variable is a store of value. The equal sign is used to assign values to variables


    The operand to the left of the = operator is the name of the variable and the operand to the right of the = operator is the value stored in the variable. For example −


    name = “Jane Doe” # a string


    Age = 30 # an integer


    Salary = 100.50 # a float


    **Data Types**


    The data stored in memory can be of many types. Python has 5 standard data types that defines the operations possible and storage;


    They include:

*   Numbers -data store for numeric values 
*   Strings -  set of characters inside double or single quotes
*   List
*   Tuples
*   Dictionary

	We will look at each in depth in the next chapters

**Python Identifiers**

A Python identifier is a name used to identify a variable, function, class, module or other object. An identifier starts with a letter A to Z or a to z or an underscore (_) followed by zero or more letters, underscores and digits (0 to 9).

Python is case sensitive hence John and john are two different variables


    Here are naming conventions for Python identifiers −



*   Class names start with an uppercase letter. All other identifiers start with a lowercase letter.
*   Starting an identifier with a single leading underscore indicates that the identifier is private.
*   Starting an identifier with two leading underscores indicates a strongly private identifier.
*   If the identifier also ends with two trailing underscores, the identifier is a language-defined special name.
5. **Basic Operators**

    Operators are the constructs which can manipulate the value of operands eg 


    3+2 =5 here 3 and 2 are operands and + is the operator


    Python supports the following operators which we will look at in depth:

*   Arithmetic Operators
*   Comparison (Relational) Operators
*   Assignment Operators
*   Logical Operators
*   Bitwise Operators
*   Membership Operators
*   Identity Operators

**Arithmetic Operators**

Python has 7 arithmetic operations which include addition(+), subtraction(-) , division( /), modulo/reminder (% ) and exponents (**)

Here are some examples you should try out:

print "5 + 2 = ",5+2	 # addition

print "5 - 2 = ", 5-2 	 # subtraction

print "5 * 2 = ", 5*2	 # multiplication

print "5 / 2 = ", 5 / 2 	# division

print "5 // 2 = ", 5 // 2.0  # floor division which truncates results

print "5 ** 2 = ", 5**2 	# power of a number /exponents

print "5 % 2 = ", 5%2  # modulus/remainder

Note: Division (/) in python2 returns a truncated decimal place and returns integer value hence need to add decimal point .0 to get the real division. This has been fixed in Python3

**Comparison (Relational) Operators**

These operators compare the values on either sides of them and decide the relation among them. They are also called Relational operators.

Here are some examples you should try out:

print "5 == 2 is  ", 5 == 2	 # returns True if the two values are equal, false otherwise

print "5 !=  2 is  ", 5  != 2 	 # returns True if the two value are not equal, false otherwise

print "5 > 2 is  ", 5 > 2 	 #  returns True if left value is greater than right value, false otherwise

print "5 < 2 is  ", 5 < 2	 # returns True if left value is less than right value, false otherwise

print "5<= 2 is  ", 5  <=  2 	#  returns True if left value is less than or equal to right value, false otherwise

print "5 >=  2 is  ", 5 >=  2  # returns True if left value is greater than or equal to right value, false otherwise

**Logical Operators**

The following are the logical operators in Python.

AND - returns true if both values are true  

OR - returns True if either of the values are true

NOT - Used to reverse the logical state of its operand 

Example

A = True

B= True

Print a and b

Print a or b

Print not( a)  

**Assignment Operators**

Assignment operators are used to assign values to the variables.

= Assign value of right side of expression to left side operand

+= Add AND: Add right side operand with left side operand and then assign to left operand

-= Subtract AND: Subtract right operand from left operand and then assign to left operand

*= Multiply AND: Multiply right operand with left operand and then assign to left operand

/= Divide AND: Divide left operand with right operand and then assign to left operand

%= Modulus AND: Takes modulus using left and right operands and assign result to left operand

**=  Exponent AND: Calculate exponent(raise power) value using operands and assign value to left operand

**Bitwise Operators**

**Membership Operators**

**in** and **not in** are the membership operators; used to test whether a value or variable is in a sequence.

in           True if value is found in the sequence

not in        True if value is not found in the sequence

**Identity Operators**

is and is not are the identity operators both are used to check if two values are located on the same part of the memory. Two variables that are equal does not imply that they are identical.



6. **Decision Making**

Decision making statements in programming languages decides the direction of flow of program execution. Decision structures evaluate multiple expressions which produce TRUE or FALSE as outcome. You need to determine which action to take and which statements to execute if outcome is TRUE or FALSE otherwise.

 Decision making statements available in python are:



*   if statement

if statement is the most simple decision making statement. It is used to decide whether a certain statement or block of statements will be executed or not i.e if a certain condition is true then a block of statement is executed otherwise not.



<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/Python-Introduction0.jpg). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/Python-Introduction0.jpg "image_tooltip")


Synatx

If condition

	Statement executed if condition is True

For example:

Age =10

If age < 18:

     print “You are below 18 years”

Print “You are over 18 years”

Output

You are below 18



*   if..else statements

We can optional use the _else_ statement with _if_ statement to execute a block of code when the condition is false.



<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/Python-Introduction1.jpg). Store image on your image server and adjust path/filename if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/Python-Introduction1.jpg "image_tooltip")


Syntax


```
if (condition):
    # Executes this block if
    # condition is true
else:
    # Executes this block if
    # condition is false
```


Example:

Age = 18

If age < 18:

   Print “You are not allowed to vote”

Else:

	Print “You are allowed to vote”

Output:

 “You are not allowed to vote”



*   nested if statements

Nested if statements means an if statement inside another if statement. 

Example:

Syntax


```
if (condition1):
   # Executes when condition1 is true
   if (condition2): 
      # Executes when condition2 is true
   # if Block is end here
# if Block is end here
```


Age = 19

If age >= 18:

	If age == 18:

		Print “You are 18 years old”

	Else:

		Print “You are older than 18”



*   if-elif-else ladder

The if statements are executed from the top down. As soon as one of the conditions controlling the if is true, the statement associated with that if is executed, and the rest of the ladder is bypassed. If none of the conditions is true, then the final else statement will be executed.

Syntax


```
if (condition):
    statement
elif (condition):
    statement
.
.
else:
    Statement
```


Example:

age = 5

if age < 18:

	print "Cannot vote"

elif age >= 18:

	print 'Can vote'

else:

	print 'Please enter a valid number'



7. **Loops**

In general, statements are executed sequentially one block of code after another. We use loops to execute a block of code several number of times.

Python provides provides the following types of loops to hande looping requirements:



*   For loop
*   While loop
*   Nestted loops

**While Loop**

In python, while loop is used to execute a block of statements repeatedly until a given a condition is satisfied. And when the condition becomes false, the line immediately after the loop in program is executed.

Syntax:

While expression:

	statement(s)

Example:

# Program to illustrate while loop

count = 0

While ( count < 9):

	Print “The count is: “,  count

	Count = count + 1

Print “Goodbye!”

Output:

 \
The block here, consisting of the print and increment statements, is executed repeatedly until count is no longer less than 9. With each iteration, the current value of the index count is displayed and then increased by 1. 


```
The count is: 0
The count is: 1
The count is: 2
The count is: 3
The count is: 4
The count is: 5
The count is: 6
The count is: 7
The count is: 8
Good bye!
```


**For Loop**

The for statement in Python has the ability to iterate over the items of any sequence, such as a list or a string.

**Syntax**


```
for iterating_var in sequence:
   statements(s)
```


**The range() function**

The built-in function range() is the right function to iterate over a sequence of numbers. It generates an iterator of arithmetic progressions.

Example to illustrate for loop using range():

for var in range(0,10):

	print var

# Another example to loop through a list

fruits = [“apple”, “banana”, “mango”]

for fruit in fruits:

	Print “Current fruit is: “, fruit

Print “Goodbye!” 

Output:

The current fruit apple

The current fruit banana

The current fruit mango

Goodbye!

**Nested Loops**

In Python, you can place one loop inside another loop. 

Syntax for loop


```
for iterating_var in sequence:
   for iterating_var in sequence:
      statements(s)
   statements(s)
```


Syntax while loop


```
while expression:
   while expression:
      statement(s)
   statement(s)
```


Example:

# Python program to illustrate nested for loops in Python 

Import sys

for i in range(1, 5): 

	for j in range(i): 

		print(i, end=' ') 

	print() 


    The print() function inner loop has end=' ' which appends a space instead of default newline. Hence, the numbers will appear in one row.


    Last print() will be executed at the end of inner for loop.

Note: You can put any type of loop inside another loop.For example a while loop can be inside a for loop and vice versa.

**Loop Control Statements**

Loop control statements change execution from its normal sequence. When execution leaves a scope, all automatic objects that were created in that scope are destroyed. Python supports the following control statements.

**Break statement**

Terminates the loop statement and transfers execution to the statement immediately following the loop.

Used for premature termination of a loop.

Example

For letter in ‘Python’:

	If letter ==  ‘h’

		Break

	Print “Current letter is:  “,  letter

Output:

Current letter is:  P

Current letter is:  y

Current letter is:  t

**Continue statement**

Causes the loop to skip the remainder of its body and immediately retest its condition prior to reiterating i.e It returns the control to the beginning of the loop.

In the example, the code will execute until it encounters letter ‘h’ then terminates and leaves the loop.

Example: To print even numbers only:

For num in range(0, 10):

	If num%2 == 0:

		Print “Found an even number: “, num

		continue

Output:

Found an even number: 0

Found an even number: 2

Found an even number: 4

Found an even number: 6

Found an even number: 8

**Pass statement**

The <code>[pass](https://docs.python.org/3/reference/simple_stmts.html#pass)</code> statement does nothing. It can be used when a statement is required syntactically but the program requires no action. For example:

while True:

	pass

 



8. **Numbers**

    Number data type stores numeric values. They are immutable data types i.e changing the value of a number data type results in a newly allocated object.


    Number objects are created when you assign a value to them. For example


    Val1 = 1


    Val2 = 15


    To delete a reference to a number object, you use the del statement as follows:


    Del val1


    Python supports the following numerical types:


    **Int (signed integer)** - they are positive or negative whole numbers withput a decimal point.


    **Float - **these represents real numbers with decipmal points eg 109.50


    **Complex numbers** -  these uses the j or J suffix to indicate the imaginary part (e.g. 3+5j).


    **Number Type Conversion**


    We use type conversion to convert one type to another in order to satisfy  certain requiremnets of an operator or a function


    Type **int(num)** to convert a number to a plain integer


    Type** float(num) **t convert a number to a decimal or floating-point numer


    Type **complex(num)** to convert a num to a complex number with real part num and an imaginary part 0


    Mathematical Function


     Python supports various Maths functions. Here are some of the common functions:


    max(num1, num2)  -  finds the largest of given arguments


    min(num1, num2) - finds the smallest of the given  arguments


    pow(num, exp) - returns the power of anumber i.e result of num**exp


    sqrt(num) - returns the squaroot of a number 


    You can checkout more maths functions supported by Python in the documentation


    **Random Number Function**


	Python defines a set of functions that are used to generate or manipulate random numbers. This particular type of functions are used in a lot of games, lotteries or any application requiring random number generation.

The following are some of the random functions:

**choice(seq) **- returns a random number from a list, tuple or strings

**randomrange([start,], stop, [,step]) **A randomly selected element from range(start, stop, step).


```
# Python code to demonstrate the working of choice() and randrange()


# importing "random" for random operations
import random


# using choice() to generate a random number from a given list of numbers.
print ("A random number from list is : ",end="")
print (random.choice([1, 4, 8, 10, 3]))


# using randrange() to generate in range from 30 to 50. The last parameter #3 is step size to skip three numbers when selecting.
print ("A random number from range is : ",end="")
print (random.randrange(30, 50, 3))
```


**random() ** - This number is used to generate a** float random number less than 1 and greater or equal to 0.**

**seed() -** Sets the integer starting value used in generating random numbers. Call this function before calling any other random module function. Returns None.


    Example:


    # An example to illustrate random number functons


    # importing "random" for random operations 


    import random 


    # using random() to generate a random number between 0 and 1 


    print ("A random number between 0 and 1 is : ", end="") 


    print (random.random()) 


    # using seed() to seed a random number 


    random.seed(5) 


    # printing mapped random number 


    print ("The mapped random number with 5 is : ", end="") 


    print (random.random()) 


    # using seed() to seed different random number 


    random.seed(7) 


    # printing mapped random number 


    print ("The mapped random number with 7 is : ", end="") 


    print (random.random()) 


    # using seed() to seed to 5 again 


    random.seed(5) 


    # printing mapped random number 


    print ("The mapped random number with 5 is : ",end="") 


    print (random.random()) 


    # using seed() to seed to 7 again 


    random.seed(7) 


    # printing mapped random number 


    print ("The mapped random number with 7 is : ",end="") 


    print (random.random()) 

**shuffle(lst)** - Randomizes the items of a list in place. Returns None.

**unfirom(a,b) **- This function is used to generate a **floating point random number between the numbers** mentioned in its arguments.** It takes two arguments, lower limit(included in generation) and upper limit(not included in generation).**


```
# Python code to demonstrate the working of
# shuffle() and uniform()
   
# importing "random" for random operations
import random
  
# Initializing list 
li = [1, 4, 5, 10, 2]
  
# Printing list before shuffling
print ("The list before shuffling is : ", end="")
for i in range(0, len(li)):
    print (li[i], end=" ")
print("\r")
  
# using shuffle() to shuffle the list
random.shuffle(li)
  
# Printing list after shuffling
print ("The list after shuffling is : ", end="")
for i in range(0, len(li)):
    print (li[i], end=" ")
print("\r")
  
# using uniform() to generate random floating number in range
# prints number between 5 and 10
print ("The random floating point number between 5 and 10 is : ",end="")
print (random.uniform(5,10))
```




9. **Strings**

Strings are amongst the most popular types in Python. They can be enclosed in single quotes (`'...'`) or double quotes (`"..."`) with the same result.

Creating strings is as simple as assigning a value to a variable. 

For example −

String1 = “Hello World”

String2 = ‘My name is John Doe’

Please note that string in single quotes cannot hold any other single quoted character in it otherwise an error arises. To overcome this error, use of double quotes is preferred, because it helps in creation of Strings with single quotes in them. Fo example:

>>> print "It doesn't help"

It doesn't help

>>> print 'It doesn't help'

  File "<stdin>", line 1

    print 'It doesn't help'

                    ^

SyntaxError: invalid syntax

Alternativelyif using single quoates, we use a slash `\`  to escape quotes:

>>> print 'It doesn\'t help'

It doesn't help

If you don’t want characters prefaced by `\` to be interpreted as special characters, you can use _raw strings_ by adding an `r` before the first quote:


```
>>> print('C:\some\name')  # here \n means newline!
C:\some
ame
>>> print(r'C:\some\name')  # note the r before the quote
C:\some\name
```


String literals can span multiple lines. One way is using triple-quotes: `"""..."""` or `'''...'''`. End of lines are automatically included in the string, but it’s possible to prevent this by adding a `\` at the end of the line. The following example:


```
print("""\
Usage: thingy [OPTIONS]
     -h                        Display this usage message
     -H hostname               Hostname to connect to
""")
```


Output:


```
Usage: thingy [OPTIONS]
     -h                        Display this usage message
     -H hostname               Hostname to connect to
```


Note the initial new line is not included.

Strings can be concatenated (glued together) with the `+` operator, and repeated with `*` eg

# Print ‘py 4 times followed by ‘thon’

>>> 'py'*4 + 'thon'

'pypypypython'

**Accessing characters in Python**

Strings can be _indexed_ (subscripted), with the first character having index 0. There is no separate character type; a character is simply a string of size one:


```
>>> word = 'Python'
>>> word[0]  # character in position 0
'P'
>>> word[3]  # character in position 5
'h'
```


Indices may also be negative numbers, to start counting from the right:


```
>>> word[-1]  # last character
'n'
>>> word[-2]  # second-last character
'o'
>>> word[-6]
'P'
```


Note that since -0 is the same as 0, negative indices start from -1.

To access substrings, use square brackets for slicing along with the index or indices to obtain your substring. For example


```
>>> word[0:2]  # characters from position 0 (included) to 2 (excluded)
'Py'
>>> word[2:5]  # characters from position 2 (included) to 5 (excluded)
'tho'
```


Note how the start is always included, and the end always excluded. This makes sure that `s[:i] + s[i:]` is always equal to `s`:


```
>>> word[:2] + word[2:]
'Python'
>>> word[:4] + word[4:]
'Python'
```


Slice indices have useful defaults; an omitted first index defaults to zero, an omitted second index defaults to the size of the string being sliced.


```
>>> word[:2]   # character from the beginning to position 2 (excluded)
'Py'
>>> word[4:]   # characters from position 4 (included) to the end
'on'
>>> word[-2:]  # characters from the second-last (included) to the end
'on'
```


One way to remember how slices work is to think of the indices as pointing _between_ characters, with the left edge of the first character numbered 0. Then the right edge of the last character of a string of _n_ characters has index _n_, for example:


```
+---+---+---+---+---+---+
 | P | y | t | h | o | n |
 +---+---+---+---+---+---+
 0   1   2   3   4   5   6
-6  -5  -4  -3  -2  -1
```


Python strings cannot be changed — they are [immutable](https://docs.python.org/3/glossary.html#term-immutable). Therefore, assigning to an indexed position in the string results in an error:


```
>>> word[2:] = 'py'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object does not support item assignment
```


If you need a different string, you should create a new one:


```
>>> word[:2] + 'py'
'Pypy'
```


The built-in function <code>[len()](https://docs.python.org/3/library/functions.html#len)</code> returns the length of a string:


```
>>> s = 'supercalifragilisticexpialidocious'
>>> len(s)
34
```


Built-in string methods

Here are some common built-in string functions used to manipulate strings. For more checkout the python [doc](https://docs.python.org/3/library/stdtypes.html#string-methods)

str.capitalize()

Capitalizes first letter of string

str.count(str, beg= 0,end=len(string))

Counts how many times str occurs in string or in a substring of string if starting index beg and ending index end are given.

str.endswith(suffix, beg=0, end=len(string))

Determines if string or a substring of string (if starting index beg and ending index end are given) ends with suffix; returns true if so and false otherwise.

str.find(str, beg=0 end=len(string))

Determine if str occurs in string or in a substring of string if starting index beg and ending index end are given returns index if found and -1 otherwise.

str.index(str, beg=0, end=len(string))

Same as find(), but raises an exception if str not found.

str.isalnum()

Returns true if string has at least 1 character and all characters are alphanumeric and false otherwise.

str.isalpha()

Returns true if string has at least 1 character and all characters are alphabetic and false otherwise.

str.isdigit()

Returns true if string contains only digits and false otherwise.

str.islower()

Returns true if string has at least 1 cased character and all cased characters are in lowercase and false otherwise.

str.isnumeric()

Returns true if a unicode string contains only numeric characters and false otherwise.

str.isspace()

Returns true if string contains only whitespace characters and false otherwise.

str.istitle()

Returns true if string is properly "titlecased" and false otherwise.

str.isupper()

Returns true if string has at least one cased character and all cased characters are in uppercase and false otherwise.

join(seq)

Merges (concatenates) the string representations of elements in sequence seq into a string, with separator string. For Example

>>> seq = ['I', 'love', 'Python']

>>> '  '.join(seq)

'I love Python'

len(string)

Returns the length of the string

str.lower()

Converts all uppercase letters in string to lowercase.

lstrip()

Removes all leading whitespace in string.

max(str)

Returns the max alphabetical character from the string str.

min(str)

Returns the min alphabetical character from the string str.

str.replace(old, new [, max])

Replaces all occurrences of old in string with new or at most max occurrences if max given.

<code>str.<strong>split</strong></code>(<em>sep=None</em>, <em>maxsplit=-1</em>)[¶](https://docs.python.org/3/library/stdtypes.html#str.split)

Return a list of the words in the string, using _sep_ as the delimiter string. For example


```
>>> '1,2,3'.split(',')
['1', '2', '3']
>>> '1,2,3'.split(',', maxsplit=1)
['1', '2,3']
>>> '1,2,,3,'.split(',')
['1', '2', '', '3', '']
```


str.startswith(str, beg=0,end=len(string))

Determines if string or a substring of string (if starting index beg and ending index end are given) starts with substring str; returns true if so and false otherwise.

strip([chars])

Return a copy of the string with the leading and trailing characters removed.


```
>>> '   spacious   '.strip()
'spacious'
>>> 'www.example.com'.strip('cmowz.')
'example'
```


str.upper()

Converts lowercase letters in string to uppercase.



10. **Lists **

Lists are the most versatile data stracture in Python. They are similar to arrays in other languages. A list is a comma separated values between square brackets. Lists may contain items of different types i.e integers, strings or another list.

Example:


```
list1 = ['physics', 'chemistry', 1997, 2000];
list2 = [1, 2, 3, 4, 5 ];
list3 = ["a", "b", "c", "d"]
```


Like strings, list indices start at 0, and lists can be indexed and sliced.


```
list1[0]:-  physics
list2[2:5]:-  [3, 4, 5] 
```


Assignment to slices is also possible, and this can even change the size of the list or clear it entirely:


```
>>> letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g']
>>> letters
['a', 'b', 'c', 'd', 'e', 'f', 'g']
>>> # replace some values
>>> letters[2:5] = ['C', 'D', 'E']
>>> letters
['a', 'b', 'C', 'D', 'E', 'f', 'g']
>>> # now remove them
>>> letters[2:5] = []
>>> letters
['a', 'b', 'f', 'g']
>>> # clear the list by replacing all the elements with an empty list
>>> letters[:] = []
>>> letters
[]
```


Lists also support operations like concatenation:


```
>>> list2 + [36, 49, 64, 81, 100]
[1, 2, 3, 4, 5 , 36, 49, 64, 81, 100]
```


Updating a List

Unlike strings, which are [immutable](https://docs.python.org/3/glossary.html#term-immutable), lists are a [mutable](https://docs.python.org/3/glossary.html#term-mutable) type, i.e. it is possible to change their content: Example


```
>>> cubes = [1, 8, 27, 65, 125]  # something's wrong here
>>> 4 ** 3  # the cube of 4 is 64, not 65!
64
>>> cubes[3] = 64  # replace the wrong value
>>> cubes
[1, 8, 27, 64, 125]
```


You can also add new items at the end of the list, by using the `append()`

shoppingList = [] 		# An empty list initialized  by empty square brackets

shoppingList.append("tomatoes")

shoppingList.append("bread")

shoppingList.append("tissue")

shoppingList.append("pens")

print shoppingList

print shoppingList[0]

print shoppingList[2]


```
Output
['tomatoes', 'bread', 'tissue', 'pens']
Tomatoes
tissue
```


Delete List Elements

To remove an item from a list given its index instead of its value we use the <code>[del](https://docs.python.org/3/reference/simple_stmts.html#del)</code> statement. This differs from the <code>pop()</code> method which returns a value. The <code>del</code> statement can also be used to remove slices from a list or clear the entire list. For example:


```
>>> a = [-1, 1, 66.25, 333, 333, 1234.5]
>>> del a[0]
>>> a
[1, 66.25, 333, 333, 1234.5]
>>> del a[2:4]
>>> a
[1, 66.25, 1234.5]
>>> del a[:]
>>> a
[]
```


<code>[del](https://docs.python.org/3/reference/simple_stmts.html#del)</code> can also be used to delete entire variables:


```
>>> del a
```


The built-in function <code>[len()](https://docs.python.org/3/library/functions.html#len)</code> is used to get the length of a list


```
>>> letters = ['a', 'b', 'c', 'd']
>>> len(letters)
4
```


To iterate over items in a list we use range() or membership operator (in).

For example to iterate and print all items in the shopping list:

shoppingList = ['tomatoes', 'bread', 'tissue', 'pens']

For item in shoppingList:

	Print item

Output

tomatoes

Bread

tissue

Pens

Using range to iterate over a list numbers


```
list2 = [1, 2, 3, 4, 5 ]
For i in range(len(list2)):
	Print "Number at index", i, "is", list[i] 

Output
```


Number at index  0 is  1

Number at index  1 is  2

Number at index  2 is  3

Number at index  3 is  4

Number at index  4 is  5


## Built-in List Functions & Methods

Python includes the following list functions −

1	cmp(list1, list2)

Compares elements of both lists.

2	len(list)

Gives the total length of the list.

3	max(list)

Returns item from the list with max value.

4	min(list)

Returns item from the list with min value.

5	list(seq)

Converts a tuple into list.

Python includes following list methods

1	list.append(obj)

Appends object obj to list

2	list.count(obj)

Returns count of how many times obj occurs in list

3	list.extend(seq)

Appends the contents of seq to list

4	list.index(obj)

Returns the lowest index in list that obj appears

5	list.insert(index, obj)

Inserts object obj into list at offset index

6	list.pop(obj=list[-1])

Removes and returns last object or obj from list

7	list.remove(obj)

Removes object obj from list

8	list.reverse()

Reverses objects of list in place

9	list.sort([func])

Sorts objects of list, use compare func if given

An example that uses most of the list methods:


```
>>> fruits = ['orange', 'apple', 'pear', 'banana', 'kiwi', 'apple', 'banana']
>>> fruits.count('apple')
2
>>> fruits.count('tangerine')
0
>>> fruits.index('banana')
3
>>> fruits.index('banana', 4)  # Find next banana starting a position 4
6
>>> fruits.reverse()
>>> fruits
['banana', 'apple', 'kiwi', 'banana', 'pear', 'apple', 'orange']
>>> fruits.append('grape')
>>> fruits
['banana', 'apple', 'kiwi', 'banana', 'pear', 'apple', 'orange', 'grape']
>>> fruits.sort()
>>> fruits
['apple', 'apple', 'banana', 'banana', 'grape', 'kiwi', 'orange', 'pear']
>>> fruits.pop()
'pear'

```



11. **Tuples**

A tuple consists of a number of values separated by commas. The difference between a list and a tuple is that tuples are immutable i.e they cannot be changed while lists are mutable.

Although not necessary, to define a tuple we  commonly encloses sequences of values in parenthesis.


```
tuple1 = 12345, 54321, 'hello!'
>>> print tuple1
(12345, 54321, 'hello!')
```


Empty tuples are constructed by an empty pair of parentheses; 


```
>>> emptyTuple = ()
```


A tuple with one item is constructed by following a value with a comma. 


```
>>> singleton = 'hello',    # <-- note trailing comma
```



## Accessing Values in Tuples


    To access values in tuple, use square brackets for slicing along with the index or indices to obtain value available at that index. For example −


```
tup1 = ('maths', 'biology', 2010, 2000);
tup2 = (1, 2, 3, 4, 5, 6, 7 );
print "tup1[0]: ", tup1[0];
print "tup2[1:5]: ", tup2[1:5];
```


When the code above is executed, it produces the following result −


```
tup1[0]:  maths
tup2[1:5]:  [2, 3, 4, 5]
```



## Updating Tuples

Tuples are immutable, this means you cannot update or change the values of tuple elements. You are able to take portions of existing tuples to create new tuples as the following example demonstrates −


```
tup1 = (12, 34.56);
tup2 = ('abc', 'xyz');

# Following action is not valid for tuples
# tup1[0] = 100;

# So let's create a new tuple as follows
tup3 = tup1 + tup2;
print tup3;
```



    When the code above  is executed, it produces the following result −


```
(12, 34.56, 'abc', 'xyz')
```


Deleting a Tuple

Since tuples are immutable you cannot remove individual elements in tuple.

To explicitly remove an entire tuple, just use the del statement. For example:

# Deleting a Tuple 

Tuple1 = (0, 1, 2, 3, 4) 

del Tuple1 

print(Tuple1) 

When the above code is executed you get an an exception error since tuple1 has been deleted and does not exist:

Traceback (most recent call last):

  File "<stdin>", line 1, in <module>

NameError: name 'Tuple1' is not defined


## Built-in Tuple Functions


    Python includes the following tuple functions −


<table>
  <tr>
   <td><strong>Sr.No</strong>
   </td>
   <td><strong>Function with Description</strong>
   </td>
  </tr>
  <tr>
   <td>1
   </td>
   <td>cmp(tuple1, tuple2)
<p>

    Compares elements of both tuples.
   </td>
  </tr>
  <tr>
   <td>2
   </td>
   <td>len(tuple)
<p>

    Gives the total length of the tuple.
   </td>
  </tr>
  <tr>
   <td>3
   </td>
   <td>max(tuple)
<p>

    Returns item from the tuple with max value.
   </td>
  </tr>
  <tr>
   <td>4
   </td>
   <td>min(tuple)
<p>

    Returns item from the tuple with min value.
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>tuple(seq)
<p>

    Converts a list into tuple.
   </td>
  </tr>
</table>




12. **Dictionary**

A dictionary as a set of _key: value_ pairs, with the requirement that the keys are unique (within one dictionary).

Dictionaries are indexed by _keys_, which can be any immutable type; strings and numbers or tuples with immutable objects. Values of a dictionary can be of any type.

Each key is separated from its value by a colon (:), the items are separated by commas, and the whole thing is enclosed in curly braces. 

Creating a Dictionary

A pair of braces creates an empty dictionary: `{}`

Dictionary can also be created by the built-in function dict(). An empty dictionary can be created by just placing to curly braces{}.

**Note – **Dictionary keys are case sensitive, same name but different cases of Key will be treated distinctly.

Example to illustrate different ways to create a Dictionary

# Creating an empty Dictionary 

Dict = {} 

print("Empty Dictionary: ") 

print(Dict) 

 

# Creating a Dictionary  with key:value pair

student_details = {'id':1234, 

		"name":"Derick Mwenda", 

		'course':'computer science',

		'year' : 3 }

print “Student details: “

print student_details

 

# Creating a Dictionary with dict() method 

Dict = dict({'id':1234, "name":"Derick Mwenda", 'course' : 'computer science', 'year' : 3 }) 

print("\nDictionary with the use of dict(): ") 

print(Dict) 

# Creating a Dictionary with each item as a Pair 

Dict = dict([(1, 'Geeks'), (2, 'For')]) 

Dict = dict([('id', 1234), ("name", "Derick Mwenda"), ('course', 'computer science'), ('year', 3)])

print("\nDictionary with each item as a pair: ") 

print(Dict) 

When the above code is executed, it produces the following result −

Empty Dictionary: 

{}

Student details:

{'course': 'computer science', 'year': 3, 'id': 1234, 'name': 'Derick Mwenda'}

Dictionary with the use of dict(): 

{'course': 'computer science', 'id': 1234, 'name': 'Derick Mwenda', 'year': 3}

Dictionary with each item as a pair: 

{'course': 'computer science', 'year': 3, 'id': 1234, 'name': 'Derick Mwenda'}

Updating a Dictionary

In Python Dictionary, Addition of elements can be done in multiple ways. 

One value at a time can be added to a Dictionary by defining value along with the key e.g. Dict[Key] = ‘Value’. For Example:

student_details = {'id': 1234, 'course': 'computer science', 'year': 3, 'name': 'Derick Mwenda'}

Student_details[“gender”] = “female” # add a new entry

Print student_details: \
When the the above code is executed it returns the fowllowing updated student details: - 

 {'id': 1234, 'course': 'computer science', 'year': 3, 'name': 'Derick Mwenda', “gender”: “female” }

You can modify an existing entry in a dictionary. For example, suppose we want to change the student course:

Student_details[‘course’] = “Software Engineering” # update an existing entry

Print student_details

The output of the above when executed will be:

 {'id': 1234, 'course': “Software Engineering”, 'year': 3, 'name': 'Derick Mwenda', “gender”: “female” }

Updating an existing value in a Dictionary can be done by using the built-in **<code>update()</code></strong> method. Nested key values can also be added to an existing Dictionary.

**Accessing elements from a Dictionary**

To access the items of a dictionary we refer to its key name. Key can be used inside square brackets.There is also a method called **get()** that will also help in acessing the element from a dictionary. For Example to access student course and gender:

Print student[‘course’]

Print student[‘gender’]

Result:

‘Software Engineering’

‘female’

Using the **get()** method to access the student name

print student_details.get('name')

Output

‘Derrick Mwenda’


## Delete Dictionary Elements


    You can either remove individual dictionary elements or clear the entire contents of a dictionary. You can also delete entire dictionary in a single operation.


    To explicitly remove an entire dictionary, just use the del statement. For example −


```
    dict = {'Name': 'Zara', 'Age': 7, 'Class': 'First'}
    del dict['Name']; # remove entry with key 'Name'
    dict.clear();     # remove all entries in dict
    del dict ;        # delete entire dictionary

    print "dict['Age']: ", dict['Age']
    print "dict['School']: ", dict['School']
```



    Output: Note that an exception is raised because after del dictdictionary does not exist any more 


```
    dict['Age']:
    Traceback (most recent call last):
       File "test.py", line 8, in <module>
          print "dict['Age']: ", dict['Age'];
    TypeError: 'type' object is unsubscriptable
```



## 
    Looping Technique

When looping through dictionaries, the key and corresponding value can be retrieved at the same time using the `items()` method.

For example to print student_details key and val

students = {'course': 'computer science', 'id': 1234, 'name': 'Derick Mwenda', 'year': 3}

for key, val in student.items():

	print key, val

Output:

course computer science

id 1234

name Derick Mwenda

year 3


## 
    Built-in Dictionary Functions & Methods


    Python includes the following dictionary functions −


<table>
  <tr>
   <td>
    <strong>Sr.No.</strong>
   </td>
   <td>
    <strong>Function with Description</strong>
   </td>
  </tr>
  <tr>
   <td>
    1
   </td>
   <td>
    cmp(dict1, dict2)
<p>

    Compares elements of both dict.
   </td>
  </tr>
  <tr>
   <td>
    2
   </td>
   <td>
    len(dict)
<p>

    Gives the total length of the dictionary. This would be equal to the number of items in the dictionary.
   </td>
  </tr>
  <tr>
   <td>
    3
   </td>
   <td>
    str(dict)
<p>

    Produces a printable string representation of a dictionary
   </td>
  </tr>
  <tr>
   <td>
    4
   </td>
   <td>
    type(variable)
<p>

    Returns the type of the passed variable. If passed variable is dictionary, then it would return a dictionary type.
   </td>
  </tr>
</table>



    Python includes following dictionary methods −


<table>
  <tr>
   <td>
    <strong>Sr.No.</strong>
   </td>
   <td>
    <strong>Methods with Description</strong>
   </td>
  </tr>
  <tr>
   <td>
    1
   </td>
   <td>
    dict.clear()
<p>

    Removes all elements of dictionary <em>dict</em>
   </td>
  </tr>
  <tr>
   <td>
    2
   </td>
   <td>
    dict.copy()
<p>

    Returns a shallow copy of dictionary <em>dict</em>
   </td>
  </tr>
  <tr>
   <td>
    3
   </td>
   <td>
    dict.fromkeys()
<p>

    Create a new dictionary with keys from seq and values <em>set</em> to <em>value</em>.
   </td>
  </tr>
  <tr>
   <td>
    4
   </td>
   <td>
    dict.get(key, default=None)
<p>

    For <em>key</em> key, returns value or default if key not in dictionary
   </td>
  </tr>
  <tr>
   <td>
    5
   </td>
   <td>
    dict.has_key(key)
<p>

    Returns <em>true</em> if key in dictionary <em>dict</em>, <em>false</em> otherwise
   </td>
  </tr>
  <tr>
   <td>
    6
   </td>
   <td>
    dict.items()
<p>

    Returns a list of <em>dict</em>'s (key, value) tuple pairs
   </td>
  </tr>
  <tr>
   <td>
    7
   </td>
   <td>
    dict.keys()
<p>

    Returns list of dictionary dict's keys
   </td>
  </tr>
  <tr>
   <td>
    8
   </td>
   <td>
    dict.setdefault(key, default=None)
<p>

    Similar to get(), but will set dict[key]=default if <em>key</em> is not already in dict
   </td>
  </tr>
  <tr>
   <td>
    9
   </td>
   <td>
    dict.update(dict2)
<p>

    Adds dictionary <em>dict2</em>'s key-values pairs to <em>dict</em>
   </td>
  </tr>
  <tr>
   <td>
    10
   </td>
   <td>
    dict.values()
<p>

    Returns list of dictionary <em>dict</em>'s values
   </td>
  </tr>
</table>




13. **Functions**

    A function is a block of organized, reusable code that is used to perform a single, related action. Functions provide better modularity for your application and a high degree of code reusing.


    Python gives you many built-in functions like print(), etc. but you can also create your own functions. These functions are called _user-defined functions._


Syntax


```
def functionname( parameters ):
   "Optional function_docstring"
   function_suite
   return [expression]
```


Note the indentation after the colon :

Example to add two numbers 

def sum(arg1, arg2):

	total = arg1 + arg2

	print "Sum of ", arg1, ' + ', arg2, ' = ', total

	Return total

# Calling the function with paramenters/arguments

sum(10,50)

When the above code is executed, it produces the following result −

Sum of  10  +  50  =  60

**Pass by Reference or pass by value?**

All parameters (arguments) in the Python language are passed by reference. It means if you change what a parameter refers to within a function, the change also reflects back in the calling function. 

For example −


```
# Function definition is here
def changeme( mylist ):
   "This changes a passed list into this function"
   mylist.append([1,2,3,4]);
   print "Values inside the function: ", mylist
   return

# Now you can call changeme function
mylist = [10,20,30];
changeme( mylist );
print "Values outside the function: ", mylist
```



    Here, we are maintaining reference of the passed object and appending values in the same object. So, this would produce the following result −


```
Values inside the function:  [10, 20, 30, [1, 2, 3, 4]]
Values outside the function:  [10, 20, 30, [1, 2, 3, 4]]
```



    Here is another example where argument is being passed by reference and the reference is being overwritten inside the called function.


```
# Function definition is here
def changeme( mylist ):
   "This changes a passed list into this function"
   mylist = [1,2,3,4]; # This would assign new reference in mylist
   print "Values inside the function: ", mylist
   return

# Now you can call changeme function
mylist = [10,20,30];
changeme( mylist );
print "Values outside the function: ", mylist
```



    The parameter _mylist_ is local to the function changeme. Changing mylist within the function does not affect _mylist_. The function accomplishes nothing and finally this would produce the following result −


```
Values inside the function:  [1, 2, 3, 4]
Values outside the function:  [10, 20, 30]
```



## Function Arguments


    You can call a function by using the following types of formal arguments −



*   Required arguments
*   Keyword arguments
*   Default arguments
*   Variable-length arguments


## Required arguments


    Required arguments are the arguments passed to a function in correct positional order. Here, the number of arguments in the function call should match exactly with the function definition.


    In this example, ou definitely need to pass two argument, otherwise it gives a syntax error as follows −

def student(name, age): 

	print(“Student name is {} and age is {}”.format(name, age))

#Calling the function

student(‘Jane’, 25)

student(25, Jane)  #inter changing the arguments 

student() # raises an error since two arguments are required

Output: Notice the order matters here and error is raise if we supply no argurments

Student name is Jane and age is 25

Student name is 25 and age is Jane

Traceback (most recent call last):

  File "<stdin>", line 1, in <module>

TypeError: student() takes exactly 2 arguments (0 given)


## Keyword arguments


    Keyword arguments are related to the function calls. When you use keyword arguments in a function call, the caller identifies the arguments by the parameter name.

This allows you to skip arguments or place them out of order because the Python interpreter is able to use the keywords provided to match the values with parameters. 

# Python program to demonstrate Keyword Arguments 

def student(name, age): 

	print(“Student name is {} and age is {}”.format(name, age))

		

# Keyword arguments				 

student(name ='Jane', age =25)	 

student(age =25, name ='Jane') 

Output: Here the order does not matter

Student name is Jane and age is 25

Student name is Jane and age is 25


## Default arguments

A default argument is an argument that assumes a default value if a value is not provided in the function call for that argument. 

def student(name, age=50): 

	print “Name: “, name

	print “Age: “, age

#Functional call

student(name = “Ruth”,age=25)

student(name= “John”)

Output: Notice default age is provided when no age is supplied

Name:  Ruth

Age:  25

Name:  John

Age:  50


## Variable-length arguments

A function can be called with an arbitrary number of arguments. Variable-length arguments are those arguments that are not specified during function definition. 

An asterisk (*) is placed before the variable name that holds the values of all non keyword variable arguments. For example

# Python program to illustrate  *args for variable number of **non-keyword** arguments eg tuple

def myFun(*argv): 

	for arg in argv: 

		print (arg) 

	

myFun('Hello', 'Welcome', 'to', 'Python') 

Keyword Arguments

Functions can also be called using keyword arguments of the form `kwarg=value`.

Double asterisks (**) are placed before the variable name that holds the values of all keyword variable arguments.

# Python program to illustrate  *kargs for variable number of keyword arguments 

def myFunc(**kwargs): 

	for key, value in kwargs.items(): 

		print ("%s == %s" %(key, value)) 

# Driver code 

myFunc(name ='John', age ='25', gender='male')	 


## The _Anonymous_ Functions

In Python, anonymous function means that a function is without a name. 

Unlike normal functions which are defined by the standard keyword **def**, anonymous functions are defined with the keyword **lambda.**

Lambda forms can take any number of arguments but return just one value in the form of an expression. They cannot contain commands or multiple expressions.

# Python code to illustrate cube of a number  using lambda function 	

cube = lambda x: x*x*x 

print(cube(5)) 

Output

125


## The _return_ Statement

The `return` statement returns with a value from a function. `return` without an expression argument returns `None`. Falling off the end of a function also returns `None`.


```
# Function definition is here
def sum( arg1, arg2 ):
   # Add both the parameters and return them."
   total = arg1 + arg2
   print "Inside the function : ", total
   return total;

# Now you can call sum function
total = sum( 10, 20 );
print "Outside the function : ", total
```



    When the above code is executed, it produces the following result −


```
Inside the function :  30
Outside the function :  30
```



## Scope of Variables


    All variables in a program may not be accessible at all locations in that program. This depends on where you have declared a variable.


    The scope of a variable determines the portion of the program where you can access a particular identifier. There are two basic scopes of variables in Python −



*   Global variables
*   Local variables


## Global vs. Local variables


    Variables that are defined inside a function body have a local scope, and those defined outside have a global scope.


    This means that local variables can be accessed only inside the function in which they are declared, whereas global variables can be accessed throughout the program body by all functions. When you call a function, the variables declared inside it are brought into scope. Following is a simple example −


```
total = 0; # This is global variable.
# Function definition is here
def sum( arg1, arg2 ):
   # Add both the parameters and return them."
   total = arg1 + arg2; # Here total is local variable.
   print "Inside the function local total : ", total
   return total;

# Now you can call sum function
sum( 10, 20 );
print "Outside the function global total : ", total
```



    When the above code is executed, it produces the following result −


```
Inside the function local total :  30
Outside the function global total :  0

```



14. **Advanced Topics**

<!-- Docs to Markdown version 1.0β17 -->
