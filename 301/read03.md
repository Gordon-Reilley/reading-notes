# Passing Functions as Props

## React Docs - lists and keys

1. The **map()** method creates a new array populated with the results of calling a provided function on every element in the calling array. **.map() returns** a new array with each element being the result of the callback function.
2. You can build collections of elements and include them in JSX using **curly braces {}** and .map().
3. Each list item needs a unique **key**.
4. The purpose of a key is to help React identify which items have changed, are added, or are removed.

## The Spread Operator

1. The **spread operator** is a useful and quick syntax for adding items to arrays, combining arrays or objects, and spreading an array out into a functionβs arguments.
2. Things that the spread operator can do:

    - Copying an array
    - Concatenating or combining arrays
    - Using Math functions
    - Using an array as arguments
    - Adding an item to a list
    - Adding to state in React
    - Combining objects
    - Converting NodeList to an array
3. An example of using the spread operator to combine two arrays:

    ```React
    [...["ππππ€ͺπ"]] // Array [ "ππππ€ͺπ" ]
    [..."ππππππ₯°ππ€©!"] // Array(9) [ "π", "π", "π", "π", "π", "π₯°", "π", "π€©", "!" ]

    const hello = {hello: "ππππ€ͺπ"}
    const world = {world: "ππππππ₯°ππ€©!"}

    const helloWorld = {...hello,...world}
    console.log(helloWorld) // Object { hello: "ππππ€ͺπ", world: "ππππππ₯°ππ€©!" }
    ```

4. An example of using the spread operator to add a new item to an array:

    ```React
    const fewFruit = ['π','π','π']
    const fewMoreFruit = ['π', 'π', ...fewFruit]
    console.log(fewMoreFruit) //  Array(5) [ "π", "π", "π", "π", "π" ]
    ```

5. An example of using the spread operator to combine two objects into one:

    ```React
    const objectOne = {hello: "π€ͺ"}
    const objectTwo = {world: "π»"}
    const objectThree = {...objectOne, ...objectTwo, laugh: "π"}
    console.log(objectThree) // Object { hello: "π€ͺ", world: "π»", laugh: "π" }
    const objectFour = {...objectOne, ...objectTwo, laugh: () => {console.log("π".repeat(5))}}
    objectFour.laugh() // πππππ
    ```

## How to Pass Functions Between Components

1. The first step that the developer does to pass functions between components was create the function where the state was.
2. The **increment function** is a function that receives a value and updates the state base on what the user does.
3. You can pass a method from a parent component into a child component by using an arrow function.
4. The child component invokes a method that was passed to it from a parent component ny using a return value.

### Sources

- <https://reactjs.org/docs/lists-and-keys.html>
- <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map>
- <https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab>
- <https://www.youtube.com/watch?v=c05OL7XbwXU>

[Back To Home](../README.md)
