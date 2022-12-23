# Read 04

## Classes and Objects

- Objects are an encapsulation of variables and functions into a single entity.
- Objects get their variables and functions from classes. Classes are essentially a template to create your objects.
- You can create multiple different objects that are of the same class(have the same variables and functions defined).
- Each object contains independent copies of the variables defined in the class.
- To access a function inside an object you use notation similar to accessing a variable.
- The __init__() function, is a special function that is called when the class is being initiated. It's used for assigning values in a class.

## Thinking Recursively

- A recursive function is a function defined in terms of itself via self-referential expressions.
-  the function will continue to call itself and repeat its behavior until some condition is met to return a result.
- All recursive functions share a common structure made up of two parts: base case and recursive case.
- When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

        - Thread the state through each recursive call so that the current state is part of the current call’s execution context 
        -  Keep the state in global scope
- A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure.

## Pytest Fixtures and Coverage

- When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code.
- But in other cases, things are a bit more complex. You'll want to have some objects available to all of your tests. Those objects might contain data you want to share across tests, or they might involve the network or filesystem. These are often known as "fixtures" in the testing world, and they take a variety of different forms.
- In pytest, you define fixtures using a combination of the pytest.fixture decorator, along with a function definition.

### Sources

- <https://www.learnpython.org/en/Classes_and_Objects>
- <https://realpython.com/python-thinking-recursively/>
- <https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage>

[Back To Home](../README.md)