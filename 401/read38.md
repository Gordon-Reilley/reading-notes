# React 2

## React Reading Notes

- In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.
- Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.
- You can use variables to store elements. This can help you conditionally render a part of the component while the rest of the output doesn’t change.
- While declaring a variable and using an if statement is a fine way to conditionally render a component, sometimes you might want to use a shorter syntax.
- You may embed expressions in JSX by wrapping them in curly braces. This includes the JavaScript logical && operator. It can be handy for conditionally including an element
- in JavaScript, true && expression always evaluates to expression, and false && expression always evaluates to false.
- Therefore, if the condition is true, the element right after && will appear in the output. If it is false, React will ignore and skip it.
- Note that returning a falsy expression will still cause the element after && to be skipped but will return the falsy expression
- Another method for conditionally rendering elements inline is to use the JavaScript conditional operator condition ? true : false.
- Just like in JavaScript, it is up to you to choose an appropriate style based on what you and your team consider more readable. Also remember that whenever conditions become too complex, it might be a good time to extract a component.
- In rare cases you might want a component to hide itself even though it was rendered by another component. To do this return null instead of its render output.
- Returning null from a component’s render method does not affect the firing of the component’s lifecycle methods.
- You can build collections of elements and include them in JSX using curly braces {}.
- Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity

### Things I want to know more about

- I'd like to know more about how react uses json, to better understand that relationship.

### Sources

- <https://reactjs.org/docs/conditional-rendering.html>
- <https://reactjs.org/docs/lists-and-keys.html>
- <https://reactjs.org/docs/forms.html>
- <https://reactjs.org/docs/lifting-state-up.html>
- <https://reactjs.org/docs/composition-vs-inheritance.html>
- <https://reactjs.org/docs/thinking-in-react.html>

[Back To Home](../README.md)