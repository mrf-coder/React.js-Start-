###  React-js
+ ComponentlifeCycle
+ Lists and Keys
+ Render Props
+ Refs
+ Events
+ High Order Components
  #### Hooks
  + useState
  + useEffect
  + useCallback
  + useReducer
  + useMemo
  + useRef
  + useContext
  + Coustom Hooks
  + Functional Components
  + JSX
  + Props vs State
  + Conditional Rendering
  + Composition vs Inheritance
  + Routing/React Router
  + Tailwind CSS
  + Component  Libraries/Shadcn UI/Material UI
  + State Management /Zustand /Jotai
  + Headless Component Libraries/Radix UI
  + FrameWork NextJs
  + API Calls/Axios
  + TypeScript
#### Rendering
   
React follows a declarative approach to rendering components, which means that developers specify what a component should look like, and React takes care of rendering the component to the screen. This is in contrast to an imperative approach, where developers would write code to manually manipulate the DOM (Document Object Model) to update the UI.

The virtual DOM (VDOM) is an important aspect of how React works. It is a lightweight in-memory representation of the DOM (Document Object Model), and it is used to optimize the rendering of components in a React application.

Components are written as JavaScript classes or functions that define a render method. The render method returns a description of what the component should look like, using JSX syntax.
When a component is rendered, React creates a virtual DOM (VDOM) representation of the component. The VDOM is a lightweight in-memory representation of the DOM, and it is used to optimize the rendering of components.
React compares the VDOM representation of the component with the previous VDOM representation (if it exists). If there are differences between the two VDOMs, React calculates the minimum number of DOM updates needed to bring the actual DOM into line with the new VDOM.
React updates the actual DOM with the minimum number of DOM updates needed to reflect the changes in the VDOM.
This process is known as reconciliation, and it is an important aspect of how React works. By using a declarative approach and a VDOM, React is able to optimize the rendering of components and improve the performance of web applications.

#### ComponentlifeCycle
React components have a lifecycle consisting of three phases: Mounting, Updating, and Unmounting along with several “lifecycle methods” that you can override to run code at particular times in the process.

It is not recommended to use lifecycle methods manually. Instead, use the useEffect hook with functional components.
#### Lists and Keys
When you render lists in React, you can use the key prop to specify a unique key for each item. This key is used to identify which item to update when you want to update a specific item.
#### Render Props
The term ‘render props’ refers to a technique for sharing code between React components using a prop whose value is a function.

A component with a render prop takes a function that returns a React element and calls it instead of implementing its own render logic.
#### Refs
Refs provide a way to access DOM nodes or React elements created in the render method.

In the typical React dataflow, props are the only way that parent components interact with their children. To modify a child, you re-render it with new props. However, there are a few cases where you need to imperatively modify a child outside of the typical dataflow. The child to be modified could be an instance of a React component, or it could be a DOM element. For both of these cases, React provides an escape hatch.
#### Events
Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

React events are named using camelCase, rather than lowercase.
With JSX you pass a function as the event handler, rather than a string.
#### High Order Components
A higher-order component (HOC) is an advanced technique in React for reusing component logic. HOCs are not part of the React API, per se. They are a pattern that emerges from React’s compositional nature.

Concretely, a higher-order component is a function that takes a component and returns a new component.

Higher-order components are not commonly used in modern React code. In order to reuse logic, React hooks are mainly used now.
  #### Hooks
  Hooks were introduced in React 16.8 and they let us use React’s features-like managing your component’s state and or performing an after effect when certain changes occur in state(s) without writing a class.
  #### useState
  useState hook is used to manage the state of a component in functional components. Calling useState returns an array with two elements: the current state value and a function to update the state.
  #### useEffect
  useEffect is a special hook that lets you run side effects in React. It is similar to componentDidMount and componentDidUpdate, but it only runs when the component (or some of its props) changes and during the initial mount.
  #### useCallback
  useCallback is a React hook that returns a memoized version of a callback function. It’s used to optimize performance by preventing unnecessary re-renders. Specifically, it helps avoid recreating functions when their dependencies haven’t changed, which can be useful when passing callbacks to child components that rely on referential equality to prevent re-rendering.
  +#### useReducer
  useReducer: An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method. (If you’re familiar with Redux, you already know how this works.)
  #### useMemo
  useMemo is a React hook that memoizes the result of a function. It is used to optimize performance by caching the result of a function and returning the cached result when the inputs to the function have not changed.
  #### useRef
  useRef is a React hook that provides a way to create a mutable reference that persists across component re-renders. It stores a value that doesn’t cause re-renders when it changes.
  #### useContext
  The useContext Hook lets us share data between components without having to pass props down through every level of the component tree. This is particularly useful when many components need to access the same data or when components are deeply nested.
  #### Coustom Hooks
  Building your own Hooks lets you extract component logic into reusable functions.
  #### Functional Components
  Functional components are some of the more common components that will come across while working in React. These are simply JavaScript functions. We can create a functional component to React by writing a JavaScript function. These functions may or may not receive data as parameters. In the functional Components, the return value is the JSX code to render to the DOM tree. Functional components can also have state which is managed using React hooks.
  #### JSX
  JSX stands for JavaScript XML. It allows writing HTML in JavaScript and converts the HTML tags into React elements.
  #### Props vs State
  Props (short for “properties”) and state are both plain JavaScript objects. While both hold information that influences the output of component render, they are different in one important way: props get passed to the component (similar to function parameters) whereas state is managed within the component (similar to variables declared within a function).
  #### Conditional Rendering
  In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application.

Conditional rendering in React works the same way conditions work in JavaScript. Use JavaScript operators like if or the conditional operator to create elements representing the current state, and let React update the UI to match them.
  #### Composition vs Inheritance
  React has a powerful composition model, and it is recommended to use composition instead of inheritance to reuse code between components.
  #### Routing/React Router
  #### Component  Libraries/Shadcn UI/Material UI
  #### State Management /Zustand /Jotai
  Application state management is the process of maintaining knowledge of an application’s inputs across multiple related data flows that form a complete business transaction — or a session — to understand the condition of the app at any given moment. In computer science, an input is information put into the program by the user and state refers to the condition of an application according to its stored inputs — saved as variables or constants. State can also be described as the collection of preserved information that forms a complete session.
  #### Headless Component Libraries/Radix UI
   ####Tailwind CSS
  #### FrameWork NextJs
  #### API Calls/Axios
  #### TypeScript
