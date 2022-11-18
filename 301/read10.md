# In memory storage

## Understanding the JavaScript Call Stack

1. What is a ‘call’?

When you invoke a function.

2. How many ‘calls’ can happen at once?

One at a time.

3. What does LIFO mean?

**LIFO**: When the call stack, operates by the data structure principle of **Last In, First Out,** it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```React
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```

5. What causes a Stack Overflow?

A **stack overflow** occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accommodate before throwing a stack error.

## JavaScript error messages

1. What is a ‘reference error’?

A **reference error** is when you try to use a variable that is not yet declared you get this type of errors.

2. What is a ‘syntax error’?

A **syntax error** occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

3. What is a ‘range error’?

a **range error** happens when you try to manipulate an object with some kind of length and give it an invalid length.

4. What is a ‘type error’?

A **type error** shows up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

5. What is a breakpoint?

A way to make your program stop at that point if the condition is met.

6. What does the word ‘debugger’ do in your code?

A **debugger** statement shows the “history” before reaching that breakpoint.

### Sources

- <https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4>
- <https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c>

[Back To Home](../README.md)
