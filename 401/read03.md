# FileIO & Exceptions

## Read & Write Files in Python

- At its core, a file is a contiguous set of bytes used to store data. 
-  This data is organized in a specific format and can be anything as simple as a text file or as complicated as a program executable.
- Files on most modern file systems are composed of three main parts:

        1. Header: metadata about the contents of the file (file name, size, type, and so on)
        2. Data: contents of the file as written by the creator or editor
        3. End of file (EOF): special character that indicates the end of the file
- When you access a file on an operating system, a file path is required. The file path is a string that represents the location of a file. It’s broken up into three major parts:

        1. Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
        2. File Name: the actual name of the file
        3. Extension: the end of the file path pre-pended with a period (.) used to indicate the file type
- When you want to work with a file, the first thing to do is to open it. This is done by invoking the open() built-in function. open() has a single required argument that is the path to the file. open() has a single return, the file object.
- It’s important to remember that it’s your responsibility to close the file. In most cases, upon termination of an application or script, a file will be closed eventually. However, there is no guarantee when exactly that will happen.
- The first way to close a file is to use the try-finally block. The second way to close a file is to use the with statement.
- There are three different categories of file objects:

        - Text files
        - Buffered binary files
        - Raw binary files

## Exceptions in Python

- Syntax errors occur when the parser detects an incorrect statement.
- Exception error occurs whenever syntactically correct Python code results in an error.
- Instead of showing the message exception error, Python details what type of exception error was encountered.
-  Python comes with various built-in exceptions as well as the possibility to create self-defined exceptions.
- We can use raise to throw an exception if a condition occurs. The statement can be complemented with a custom exception.
- Instead of waiting for a program to crash midway, you can also start by making an assertion in Python. We assert that a certain condition is met. If this condition turns out to be True, then that is excellent! The program can continue. If the condition turns out to be False, you can have the program throw an AssertionError exception.
- The try and except block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.
- Key takeaways:

        - A try clause is executed up until the point where the first exception is encountered.
        - Inside the except clause, or the exception handler, you determine how the program responds to the exception.
        - You can anticipate multiple exceptions and differentiate how the program should respond to them.
        - Avoid using bare except clauses.
- In Python, using the else statement, you can instruct a program to execute a certain block of code only in the absence of exceptions.
- Imagine that you always had to implement some sort of action to clean up after executing your code. Python enables you to do so using the finally clause.

### Summary

- raise allows you to throw an exception at any time.
- assert enables you to verify if a certain condition is met and throw an exception if it isn’t.
- In the try clause, all statements are executed until an exception is encountered.
- except is used to catch and handle the exception(s) that are encountered in the try clause.
- else lets you code sections that should run only when no exceptions are encountered in the try clause.
- finally enables you to execute sections of code that should always run, with or without any previously encountered exceptions.

### Sources

- <https://realpython.com/read-write-files-python/>
- <https://realpython.com/python-exceptions/>
- <https://realpython.com/python-exceptions/>
- <https://realpython.com/quizzes/read-write-files-python/>

[Back To Home](../README.md)