# Combined Reducers

## [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)




### Why create multiple reducers?

Creating multiple reducers in a Redux-based application is a common practice to manage different parts of your application's state separately and keep the codebase more organized and maintainable. 

**Modularity and Maintainability:** By creating multiple reducers, you can break down the complex application state into smaller, manageable pieces. Each reducer is responsible for a specific part of the state,

**Separation of Concerns:** Different parts of your application often have distinct state requirements. For example, an e-commerce app might have separate reducers for managing products, user authentication, shopping cart, and order history.

**Reusability:** Reducers can be reused across different parts of your application or even in different projects, promoting code reusability.

### How would you combine multiple reducers?

In Redux, you typically use the **combineReducers** function to combine multiple reducers into a single root reducer.

### How will you manage state as an immutable object? why?

To manage state as an immutable object in JavaScript, you should follow certain practices and techniques. 

1. **Use Object Spread (for Objects) and Array Spread (for Arrays):** 

When you need to make changes to an object or an array, create a new object or array by spreading the properties or elements of the existing one and make your modifications. This ensures that you don't modify the original data.

![example](./img/Screenshot%202023-09-11%20124455.png)

2. **Avoid Direct Mutation:**

Never modify the properties or elements of an object or array directly. This includes using methods like push, pop, splice, and Object.assign, which modify the original data.

![example](./img/Screenshot%202023-09-11%20124709.png)


3. **Use Immutability Helpers (if necessary)**

![example](./img/Screenshot%202023-09-11%20124834.png)

4. **Deep Cloning (with caution):**


## [Redux Docs: Using Combined Reducers](https://redux.js.org/usage/structuring-reducers/using-combinereducers/)




### combineReducers is a utility function to simplify the most common use case when writing ___ _____ .

when writing Redux reducers. Its primary purpose is to help manage different parts of your application's state in a more organized and modular way.


### Explain how combineReducers assembles the new state tree.

When you use combineReducers, it assembles the new state tree by calling each individual reducer you provided as arguments to it

![example](./img/Screenshot%202023-09-11%20125933.png)

### How would you define initial state in an app using combineReducers?

To define the initial state in an app using combineReducers, you typically provide an initial state for each individual reducer as the default parameter in their function definitions. Here's an example:

![example](./img/Screenshot%202023-09-11%20131712.png)

## [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)





### Why will you want to split your reducing functions as your app becomes more complex?

 to improve maintainability, organization, and separation of concerns

### The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.

The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to Redux's createStore function.

![example](./img/Screenshot%202023-09-11%20132859.png)


### What is a popular convention when naming reducers?

A popular convention when naming reducers is to use the "reducer" suffix. For example, if you have a reducer responsible for managing the user's authentication state, you might name it **authReducer**