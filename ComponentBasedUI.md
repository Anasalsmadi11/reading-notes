# Component Based UI

## [React Quick Start](https://react.dev/learn)



### What are the building blocks of a React app?

1. Components
1. JSX (JavaScript XML)
1. State
1. Props 
1. Virtual DOM (Document Object Model)
1. Lifecycle Methods (for class components)
1. Hooks (for functional components)
1. Router (React Router)
1. Styling

### What is the difference between an HTML element and a React component?

|React Component|HTML Element|
|-|-|
|A React component is a JavaScript function or class that generates UI elements.|An HTML element is a basic building block of a web page's structure and content.|
|It's defined using JSX (JavaScript XML), a syntax extension that combines JavaScript and HTML-like syntax|It's defined using HTML tags, like <div>, <p>, <img>, etc.
|
|Components can have internal state, manage props (data passed from parent components), and handle user interactions.
|HTML elements define the structure and content of a web page, but they don't encapsulate behavior or logic.
|
|Components can have internal state, manage props (data passed from parent components), and handle user interactions.
|HTML elements are static and don't easily allow for dynamic updates or interactivity without additional JavaScript code.
|

### What is JSX and why do we use it?

JSX stands for JavaScript XML. It is a syntax extension used with React

Here are some key points about JSX and why it's used:

* Combining JavaScript and HTML
* Readability
* Component-Based Architecture
* Enhanced Tooling

### Describe the process of embedding JavaScript expressions in JSX.

Embedding JavaScript expressions in JSX involves placing the JavaScript code within curly braces {} directly inside the JSX code. This allows you to dynamically insert values, evaluate expressions, and execute JavaScript logic within your JSX-rendered components. 

### Does React or JSX have any special features for iteration or conditional logic?

Yes, both React and JSX have special features for iteration and conditional logic that make it easier to work with dynamic UIs.

### How does React know to respond to a user’s inputs?

React responds to a user's inputs through a combination of event handling and state management.

### What word indicates that a React component manages data with a Hook?


The word that indicates that a React component manages data with a Hook is "Hook" itself.React, a Hook is a special function that allows you to "hook into" React state and lifecycle features from functional components.

some commonly used data-managing Hooks include:

1. useState: This Hook allows functional components to manage state by providing a state variable and a function to update that state.

1. useEffect: This Hook enables you to perform side effects (e.g., data fetching, DOM manipulation) in functional components. It takes a function that will be executed after rendering and can be used to manage component lifecycle aspects.

1. useContext: This Hook allows you to consume data from a React context, which provides a way to share data across the component tree without having to pass props manually at each level.

1. useReducer: This Hook is an alternative to useState for managing more complex state logic

### How can two react components share data?

Two React components can share data by using a combination of props, state lifting, context, and other communication patterns 

Here are some common methods to achieve data sharing between components:

1. Props 
1. State Lifting (Child-to-Parent Communication)
1. State Lifting (Child-to-Parent Communication)
1. Context API
1. Redux (or other State Management Libraries)
1. Event Bus or Pub-Sub
1. Custom Hooks

## [Render and Commit](https://react.dev/learn)




### What are the three steps of refreshing a React UI?

Refreshing a React UI involves updating the view to reflect changes in the component's state or props. The process of refreshing a React UI typically involves three main steps:

1. State or Props Update
1. Component Re-rendering
1. DOM Update

### How do you trigger updates to a component after the initial render?

In React, you can trigger updates to a component after the initial render by modifying its state or props. React will automatically re-render the component whenever its state or props change. 

### Does React recreate DOM nodes on every rerender?

No, React does not recreate all DOM nodes on every re-render. Instead, React uses a virtual DOM (VDOM) and a process called **"reconciliation"** to efficiently update the actual DOM only with the necessary changes.

### After React has updated the DOM, what still needs to happen before the user sees the change?

After React has updated the DOM, there are a few steps that need to occur before the user sees the change on the screen:


* Reflow and Repaint
* Style Calculation
* Display Update