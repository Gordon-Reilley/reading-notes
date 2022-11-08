# State and Props

## React lifecycle

1. The **render** happens before the **componentDidMount** according to the diagram.
2. The very first thing to happen in the lifecycle of React is the **mounting phase**.
3. The following things are in the order that they happen:

    - Constructor
    - Render
    - componentDidMount
    - React Updates
    - componentWillUnmount
4. **componentDidMount** method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here.

## React State Vs Props

1. Types of things can you pass in **props** are initial counts, labels, titles that don't change, and numbers.
2. The big difference between props and state are that props are handled outside of the component, and states are handled inside of that component.
3. We re-render our application when every time the state changes.
4. Some examples of things that we could store in state are:

    - updated values
    - changing labels
    - user information
    - counters
    - strings
    - numbers

### Sources

- <https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093>
- <https://www.youtube.com/watch?v=IYvD9oBCuJI>

[Back To Home](../README.md)
