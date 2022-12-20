# Read: Class 02

## Readings

1. **In Tests We Trust - TDD with Python**

    - Unit tests are some pieces of code to exercise the input, the output and the behavior of your code. You can write them anytime you want. But Test-Driven Development is a strategy to think (and write!) tests first.
    - There are some details to pay attention. The first one is the test name. The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.
    - The test file name should follow the same name of module name.
    - Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.

      - Arrange: you need to organize the data needed to execute that piece of code (input);
      - Act: here you will execute the code being tested (exercise the behaviour);
      - Assert: after executing the code, you will check if the result (output) is the same as you were expecting.
    - The cycle is made by three steps:

      - Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)
      - Write the feature and make the test pass! (you can dance after that)
      - Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)
2. **If name equals main**

      - If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”.
      - If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 
      - A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 
         ```` Python
         # Python program to execute
         # main directly
         print ("Always executed")
         
         if __name__ == "__main__":
             print ("Executed when invoked directly")
         else:
             print ("Executed when imported")
         ````
      - All the code that is at indentation level 0 [Block 1] gets executed. Functions and classes that are defined are, well, defined, but none of their code runs. 
      - Here, as we executed script.py directly __name__ variable will be __main__. So, code in this if block[Block 2] will only run if that module is the entry point to your program. 
      - Thus, you can test whether your script is being run directly or being imported by something else by testing __name__ variable. 
      - If script is getting imported by some other module at that time __name__ will be module name.
3. **Recursion**

      - The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called a recursive function.
      -  Using a recursive algorithm, certain problems can be solved quite easily. Examples of such problems are Towers of Hanoi (TOH), Inorder/Preorder/Postorder Tree Traversals, DFS of Graph, etc.
      - A recursive function solves a particular problem by calling a copy of itself and solving smaller sub-problems of the original problems.
      - It is essential to know that we should provide a certain case in order to terminate this recursion process. So we can say that every time the function calls itself with a simpler version of the original problem.
      - Recursion is an amazing technique with the help of which we can reduce the length of our code and make it easier to read and write.
      - Base condition is needed to stop the recursion otherwise infinite loop will occur.
      - Recursion uses more memory, because the recursive function adds to the stack with each recursive call, and keeps the values there until the call is finished.
      - The recursive function uses LIFO (LAST IN FIRST OUT) Structure just like the stack data structure.
      - In the recursive program, the solution to the base case is provided and the solution to the bigger problem is expressed in terms of smaller problems. 
      - A function fun is called direct recursive if it calls the same function fun. A function fun is called indirect recursive if it calls another function say fun_new and fun_new calls fun directly or indirectly.

### Sources

- <https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932>
- <https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/>
- <https://www.geeksforgeeks.org/introduction-to-recursion-data-structure-and-algorithm-tutorials/>
- <https://www.youtube.com/watch?v=Mv9NEXX1VHc>
- <https://realpython.com/courses/python-modules-packages/>

[Back To Home](../README.md)
