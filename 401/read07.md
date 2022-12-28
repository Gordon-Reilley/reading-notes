# Ten Thousand 2

## Python Scope

### Global

- You can access or reference global names from any place in your code, but they can be modified or updated from within the global Python scope.
- You can access local names only from inside the local Python scope they were created in or from inside a nested function, but you can’t access them from the global Python scope or from other local scopes.
- When you try to assign a value to a global name inside a function, you create a new local name in the function scope.
- You can use a **global statement** to define a list of names that are going to be treated as global names.
- The statement consists of the global keyword followed by one or more names separated by commas. You can also use multiple global statements with a name (or a list of names). All the names that you list in a global statement will be mapped to the global or module scope in which you define them.
- The use of global is considered bad practice in general. If you find yourself using global to fix problems like the one above, then stop and think if there is a better way to write your code.
- You can also use a global statement to create lazy global names by declaring them inside a function.
- Finally, it’s worth noting that you can use global from inside any function or nested function and the names listed will always be mapped to names in the global Python scope.
### Nonlocal

- Nonlocal names can be accessed from inside nested functions, but they can’t be modified or updated from there.
- If you want to modify them, then you need to use a nonlocal statement.
- With a nonlocal statement, you can define a list of names that are going to be treated as nonlocal.
- The nonlocal statement consists of the nonlocal keyword followed by one or more names separated by commas. These names will refer to the same names in the enclosing Python scope.
- Unlike global, you can’t use nonlocal outside of a nested or enclosed function. To be more precise, you can’t use a nonlocal statement in either the global scope or in a local scope.
- In contrast to global, you can’t use nonlocal to create lazy nonlocal names. Names must already exist in the enclosing Python scope if you want to use them as nonlocal names. This means that you can’t create nonlocal names by declaring them in a nonlocal statement in a nested function.
### Sources

- <https://realpython.com/python-scope-legb-rule/>
- <https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Program_Example_1_3>

[Back To Home](../README.md)