#  Redux - Additional Topics

## [Redux Toolkit (RTK)](https://redux-toolkit.js.org/introduction/getting-started)




### What concerns are addressed by Redux Toolkit?


Redux Toolkit addresses several concerns related to using Redux in a JavaScript or React application:

* Boilerplate Reduction: Redux by itself can involve writing a significant amount of boilerplate code to set up actions, action types, reducers, and store configuration.

* Immutability: Redux Toolkit encourages the use of immutable state updates, which helps prevent common bugs related to mutable state in Redux. 

* Simplified Redux Configuration: It provides simplified and opinionated configuration options for creating a Redux store, allowing you to set up a store with sensible defaults without the need for extensive manual configuration.

* Reducers and Actions: Redux Toolkit introduces createSlice(), which simplifies the process of creating reducers and action creators. 
* Middleware Integration: It seamlessly integrates middleware, such as Thunk or Saga, into your Redux store, simplifying the middleware setup process.

### What does configureStore() do?

configureStore(): wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

### How would I use createSlice()?

createSlice(): accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.


## [MobX](https://mobx.js.org/getting-started.html)





### What is Mobx?

MobX is a simple, scalable and battle tested state management solution.

### How does MobX make it “impossible” to produce an inconsistent state?


MobX reduces the chances of inconsistent states by automatically tracking dependencies, providing transactions, enforcing strict mode, and handling garbage collection, making it less error-prone compared to manual state management. However, it doesn't make inconsistencies "impossible" if used improperly.

### How would we build a reactive user interface?

1. Identify the parts of your UI that need to be reactive.

1. Use MobX to create and manage your application's state, defining observables and actions to update that state.

1. React to changes in your observables by using MobX reactions (e.g., autorun or observer).

1. Implement user interactions that trigger actions to modify observables.

1. Define your UI components to render based on the state stored in MobX observables.

1. Test your reactive UI, ensuring that changes to state result in the expected updates to your UI components.

1. Optimize performance by using memoization and only updating the UI when necessary.

1. Implement error handling and real-time updates as needed.