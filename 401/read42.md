# Pythonisms

## Dunder Methods

- In Python, special methods are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores, for example `__init__` or `__str__`.
- As it quickly became tiresome to say under-under-method-under-under Pythonistas adopted the term “dunder methods”, a short form of “double under.”
- Dunder methods let you emulate the behavior of built-in types. For example, to get the length of a string you can call len('string'). But an empty class definition doesn’t support this behavior out of the box
- This elegant design is known as the Python data model and lets developers tap into rich language features like sequences, iteration, operator overloading, attribute access, etc.
- Various dunder methods that unlock the following language features:
  - Initialization of new objects
  - Object representation
  - Enable iteration
  - Operator overloading (comparison)
  - Operator overloading (addition)
  - Method invocation
  - Context manager support (with statement)

## Iterators

- Iterators are so useful in Python: They allow you to write pretty for-in loops and help you make your code more Pythonic and efficient.
- Objects that support the `__iter__` and `__next__` dunder methods automatically work with for-in loops.
- The for-in was just syntactic sugar for a simple while loop:
  - It first prepared the repeater object for iteration by calling its `__iter__` method. This returned the actual iterator object.
  - After that, the loop repeatedly calls the iterator object’s `__next__` method to retrieve values from it.
-  `__iter__` and `__next__` can be called with Python’s built-in functions iter() and next(). Internally these built-ins invoke the same dunder methods, but they make this code a little prettier and easier to read by providing a clean “facade” to the iterator protocol.
- Python offers these facades for other functionality as well. For example, len(x) is a shortcut for calling `x.__len__`. Similarly, calling iter(x) invokes `x.__iter__` and calling next(x) invokes `x.__next__`.
- Generally it’s a good idea to use the built-in facade functions rather than directly accessing the dunder methods implementing a protocol. It just makes the code a little easier to read.

## Generators

- Generators look like regular functions but instead of using the `return` statement, they use `yield` to pass data back to the caller.
- Generators look like normal functions, but their behavior is quite different. For starters, calling a generator function doesn’t even run the function. It merely creates and returns a generator object.
- The code in the generator function only executes when `next()` is called on the generator object.
- Whereas a return statement disposes of a function’s local state, a yield statement suspends the function and retains its local state.
- You’ll find that for most types of iterators, writing a generator function will be easier and more readable than defining a long-winded class-based iterator.
- Generator functions are syntactic sugar for writing objects that support the iterator protocol. Generators abstract away much of the boilerplate code needed when writing class-based iterators.
- The yield statement allows you to temporarily suspend execution of a generator function and to pass back values from it.
- Generators start raising StopIteration exceptions after control flow leaves the generator function by any means other than a yield statement.

### Things I want to know more about

- I'd like to know more about .

### Sources

- <https://dbader.org/blog/python-dunder-methods>
- <https://dbader.org/blog/python-iterators>
- <https://dbader.org/blog/python-generators>
- <https://realpython.com/lessons/what-are-python-generators/>

[Back To Home](../README.md)