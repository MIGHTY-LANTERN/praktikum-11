# praktikum-11
Exception Handling
Exception is an error that occurs when the program execution process is running,
This error will cause the program to end abnormally.
Handling
File handling is an important part of any application.
Assertion
Assertion is the reasonableness of a program that you can enable/disable when you finish running the program.

The Assert Statement
When it finds a statement, Python evaluates the accompanying expression, which is hopefully correct. If the expression is incorrect, Python throws an AssertionError exception.
The syntax for the statement is :
assert Expression[, Arguments]
If the statement fails, Python uses the ArgumentExpression ArgumentExpression as the argument argument for the AssertionError AssertionError. AssertionError Exceptions AssertionError exceptions can be caught and handled like any other exception using try- except statements, but if left unchecked, they will stop the program and generate a backtrace.

Example
Here is a function that converts the temperature from degrees Kelvin to degrees Fahrenheit.Since zero degrees Kelvin is cold, the function function stores it if it sees a negative negative temperature.
When the code below is run, it produces the following results: gambar
Handling Exceptions
If you have some suspicious code that may issue an exception, you can keep your program put the suspicious code in the try: block. After try: block, include an except: statement included: statement, followed by a code block that handles the problem as gracefully as possible.

Example
These examples open the file, write the contents of the file, and exit safely because there is no problem
When the code below is run, it produces the following results: gambar
This example tries to open a file for which you do not have write permissions, thus creating an exception file
When the code below is run, it produces the following results: gambar
Phases except without Exceptions
You can also use an exception statement without an exception defined as follows:
try:
You do your operations here;
......................
except:
If there is any exception, then execute this block.
......................
else:
If there is no exception then execute this block.
A try-except statement of this type catches all exception exceptions that occur. Using experiments such as try-expect statements is not considered good programming practice, as they catch all exceptions but do not make the programmer identify the possible cause of the problem occurring

Clauses except with Various Exceptions
You can also use the same exception statement to handle multiple exceptions as follows:
try:
You do your operations here;
......................
except(Exception1[, Exception2[,...ExceptionN]]]):
If there is any exception from the given exception list,
then execute this block.
......................
else:
If there is no exception then execute this block.
End-and-error clause
Example
If you do not have permission to open the file in write write mode, then this will produce the following results: 9 4 1
The same example can be written cleaner as follows: gambar When an exception is thrown into the try block, the execution immediately proceeds to the end of the block. After all statements in the block are finally executed, exceptions are raised again and handled in the statement unless there is a next layer higher than the experiment-except statement.
Exception Arguments
Example
Here's an example for one exception
When the code below is run, it produces the following results: gambar
Throwing an Exception
Example
Exceptions can be strings, classes, or objects. Most of the exceptions are exceptions from core Python raises are classes, with argument=arguments that are derivatives of the class. Defining new exceptions is fairly easy and can be done as follows: gambar
User-Defined Exceptions
Python also lets you create your own exceptions by deriving classes from the standard built-in exceptions.
Here are examples related to RuntimeError. Here, a class is created that is a subclass of the RuntimeError subclass. This is useful when you need todisplay a more specific view of information when e exception is caught.
In the test block, a user-defined exception is raised and caught in the exclude block. The variable e is used to create an instance of the Networkerror class. gambar
hihi ^^
