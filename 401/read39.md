# React 3

## NextJs

- Important details to consider:
- Code has to be bundled using a bundler like webpack and transformed using a compiler like Babel.
- You need to do production optimizations such as code splitting.
- You might want to statically pre-render some pages for performance and SEO. You might also want to use server-side rendering or client-side rendering.
- You might have to write some server-side code to connect your React app to your data store.
- Assets
- Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

## React Context for Beginners

- React Context is a feature in React that provides a way to pass data through the component tree without having to pass props down manually at every level.
- It allows components to access data that is defined at a higher level in the component tree, making it available to all components within the tree.
- React Context is created using the React.createContext method, which returns an object with a Provider and a Consumer.
- The Provider is used to store the data that should be made available to the components, and the Consumer is used to access the data from the Provider.
- The Provider can be wrapped around multiple components in the tree to make the data available to all of them.
- React Context can be used for various purposes, including managing global state, providing themes, and handling authentication.
- React Context should be used judiciously, as it can make the codebase complex and harder to debug if not used properly.
- It is best used for data that is not updated often such as (theme data like dark mode, user data like currently authenticated user, location specific data like language)


### Things I want to know more about

- I'd like to know more about if there is a better way to share states or data that does need to be updated often between components.

### Sources

- <https://nextjs.org/learn/basics/create-nextjs-app>
- <https://www.freecodecamp.org/news/react-context-for-beginners/>

[Back To Home](../README.md)