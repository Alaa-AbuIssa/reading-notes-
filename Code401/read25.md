# Context API

## Review, Research, and Discussion

* 1. Describe use cases `useState()` vs `useReducer()`

- *useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.*

- *Although useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.*

- *useReducer lets you avoid passing down callbacks through different levels of your component, instead allowing you to pass a provided dispatch function, which in turn will improve performance for components that trigger deep updates.*

- *the useState updater function is newly called on each render. What it means is that when you have a complex logic to update state, you simply won’t use the setter directly to update state; instead, you will write a complex function, which in turn would call the setter with updated state.*

* 2. Why do custom hooks need the use prefix?

*Custom hooks are normal JS functions, named with the prefix ‘use’, that can use hooks inside of it and contain a common stateful logic to be reused in other components.*

* 3. What do custom hooks usually do?
*Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.*

* 4. Using any list of custom hooks, research and name one that you think will be useful in your applications
***useScript React hook to dynamically load an external script and know when its loaded***

*useScript is a hook for loading (and notifying when they’re loaded) external scripts, dynamically.*

***use-mouse-action***
*A library with three React hooks for listening to mouse events on an element or JSX element. useMouseAction: This is used to register mouse actions on an element. useMouseDown: This is used to register a mouse down event on an element. useMouseUp: This registers a mouse up event on an element.*


* 5. Describe how a hook that fetches API data might work
*Put the fetchData function above in the useEffect hook and call it, like so: useEffect(() => { const url = "https://api.adviceslip.com/advice (Links to an external site.)"; const fetchData = async () => { try { const response = await fetch(url); const json = await response. json(); console. log(json); } catch (error) { console*


## Document the following Vocabulary Terms
**reducer**:
*A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently*

## preperation material (Links to an external site.)
React.createContext: Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree. (Links to an external site.)
Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. (Links to an external site.)

```
class MyClass extends React.Component {
  componentDidMount() {
    let value = this.context;
    /* perform a side-effect at mount using the value of MyContext */
  }
  componentDidUpdate() {
    let value = this.context;
    /* ... */
  }
  componentWillUnmount() {
    let value = this.context;
    /* ... */
  }
  render() {
    let value = this.context;
    /* render something based on the value of MyContext */
  }
}
MyClass.contextType = MyContext;
```

### Caveats 
*Because context uses reference identity to determine when to re-render, there are some gotchas that could trigger unintentional renders in consumers when a provider’s parent re-renders. For example, the code below will re-render all consumers every time the Provider re-renders because a new object is always created for value*
### context api
*Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree; and its designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.*

### React.createContext:
*Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.*

*The defaultValue argument is only used when a component does not have a matching Provider above it in the tree. This default value can be helpful for testing components in isolation without wrapping them. Note: passing undefined as a Provider value does not cause consuming components to use defaultValue*.