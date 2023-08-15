# useState()

## [Thinking in React](https://react.dev/learn/thinking-in-react)

### Summarize the five steps of thinking in react.
1. Start with a Mock
1. Build a Static Version 
1. Identify the Minimal (but complete) Representation of UI State
1. Where to Hold State
1. Add Inverse Data Flow

## [State: A Component’s Memory](https://react.dev/learn/state-a-components-memory)




### What is one reason a local variable isn’t sufficient for managing a React component?

One reason a local variable isn't sufficient for managing a React component is that local variables do not trigger re-renders. React components need to respond to changes in data and update their UI accordingly. Using local variables alone would not automatically update the component's rendering when the variable changes,

### What is the argument to the useState hook, and what are the two parts of its return array?

It takes an initial value as an argument and returns an array with two elements:

**State Variable**: The first element of the returned array is the state variable itself, which holds the current state value.

**State Updater Function**: The second element of the returned array is a function that allows you to update the state. This function is used to modify the state variable. 


### How can Component A access state from Component B?

Components in React should communicate and share state through props, lifting state up (if they have a common ancestor), or by using the Context API for broader state sharing. Direct state access between unrelated components is avoided to maintain a clean and organized architecture.