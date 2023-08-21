#  Advanced State with Reducers

[Extracting State Logic into a Reducer](https://react.dev/learn/extracting-state-logic-into-a-reducer)




### What is the motivation for adding a reducer?
The useReducer hook in React is an alternative to the more commonly used useState hook for managing component state. It's particularly useful when the state transitions are more complex and involve multiple actions that can lead to state changes. 


### What are actions in the context of a reducer? How are they different than setting state directly?


In the context of a reducer, actions are plain JavaScript objects that describe changes you want to make to the state. They typically have a type property that indicates the type of action being performed,


### What common list operation is useReduce named for, and why?

The useReducer hook in React is named after the common list operation known as "reduction" or "fold."

### When should you switch from useState to useReducer?

The decision to switch from useState to useReducer in React depends on the complexity of your state management and the needs of your application. While both hooks are used for managing state, they have different use cases and can be more suitable for different scenarios. 