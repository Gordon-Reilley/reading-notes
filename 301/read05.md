# Putting it all together

## React Docs - Thinking in React

1. What is the single responsibility principle and how does it apply to components?
The single responsibility principle is the principle that a component should only do one thing.
2. What does it mean to build a ‘static’ version of your application?
**Static applications** and websites render in the user's browser without the need for server side processing, this means that all the rendering of HTML, CSS, and JavaScript is done on the client side, rather then relying on server side technologies.
3. Once you have a static application, what do you need to add?
You have to add a **state** to the application.
4. What are the three questions you can ask to determine if something is state?

    - Is it passed in from parents via props?
    - Does it remain unchanged over time?
    - Can you compute it based on any other states or props in your component?

5. How can you identify where state needs to live?

    - Identify every component that renders something based on that state.
    - Find a common owner component
    - Find another component higher up in the hierarchy should own the state.

## Higher-Order Functions

1. What is a “higher-order function”?
Higher order functions are functions that take in other functions as arguments and return them.
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
It's returning a value greater than n.
3. Explain how either map or reduce operates, with regards to higher-order functions.
**.map** is a method that can be used on arrays to iterate through each index of the array and apply some function in order to return a new array.

### Sources

- <hhttps://reactjs.org/docs/thinking-in-react.html>
- <https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK>

[Back To Home](../README.md)
