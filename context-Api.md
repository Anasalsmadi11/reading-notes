# Context API

## [Choosing the State Structure](https://react.dev/learn/choosing-the-state-structure)

### Summarize the five principles for structuring state.

1. Group related state. If you always update two or more state variables at the same time, consider merging them into a single state variable.

1. Avoid contradictions in state. When the state is structured in a way that several pieces of state may contradict and “disagree” with each other, you leave room for mistakes. Try to avoid this.
1. Avoid redundant state. If you can calculate some information from the component’s props or its existing state variables during rendering, you should not put that information into that component’s state.
1. Avoid duplication in state. When the same data is duplicated between multiple state variables, or within nested objects, it is difficult to keep them in sync. Reduce duplication when you can.
1. Avoid deeply nested state. Deeply hierarchical state is not very convenient to update. When possible, prefer to structure state in a flat way.

## [Passing State Deeply with Context](https://react.dev/learn/passing-data-deeply-with-context)




### What problem do Contexts aim to solve?

Usually, you will pass information from a parent component to a child component via props. But passing props can become verbose and inconvenient if you have to pass them through many components in the middle, or if many components in your app need the same information. Context lets the parent component make some information available to any component -no matter how deep - without passing it explicitly through props.



### What is one technique to try before useContext?

efore using the useContext hook in React, you might consider using the "prop drilling" technique. Prop drilling involves passing data from a higher-level component down to a lower-level component through its props

### What hook complements useContext for complex applications?

In complex React applications, the useReducer hook often complements the useContext hook when managing state. While useContext provides a way to share state across components without having to pass props through intermediary components (prop drilling), useReducer helps manage state transitions in a more structured and predictable manner