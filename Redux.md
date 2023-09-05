# Application State with Redux

## [Dan Abramov Redux Tutorials](https://egghead.io/courses/fundamentals-of-redux-course-from-dan-abramov-bd5cc867)




### What is the first principle of Redux?

In Redux, the application's entire state is stored in a single JavaScript object known as the "store." This means that all data that your application needs to manage and display is centralized in one place, making it the single source of truth for your application's state.

### what is a store and what do we use our reducers for within that store?

The store in Redux is a central and immutable JavaScript object that holds the entire state of your application. It serves as the single source of truth for your application's data.
The store contains the current state of your application, and you can access this state by querying the store. However, you cannot modify the store's state directly; instead, you use actions and reducers to update the state.


* Reducers are JavaScript functions that specify how the application's state changes in response to actions.

* Reducers take two arguments: the current state (which is typically provided as a default parameter) and an action object.

* They return a new state based on the action, ensuring that the state remains immutable.

* Reducers are pure functions, meaning they do not have any side effects, and the same input always produces the same output.

### Name three Redux store methods given to us by createStore and describe their use.

### getState():


* The getState() method is used to retrieve the current state of the Redux store. It returns the current state object, allowing you to access the entire state tree.

* Use this method when you need to access and read the application's state.

### dispatch(action):

* The dispatch(action) method is used to dispatch actions to the store. Actions are plain JavaScript objects that describe what should happen in your application. 

* Use this method to initiate changes to the state. When you dispatch an action, it is processed by the reducers, which update the state accordingly.


### Explain to a non-technical recruiter what combineReducers() does and why it is useful.

combineReducers() is like a manager for organizing and coordinating different parts of your application's data. It helps keep your code clean and organized by allowing you to manage separate pieces of data with separate functions, making your code easier to understand and maintain.