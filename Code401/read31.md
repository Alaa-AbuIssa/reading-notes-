# Redux - Combined Reducers


## Review, Research, and Discussion

1. Why choose Redux instead of the Context API for global state?

* Context API is great for small applications where state changes are minimal but Redux is better for large applications where there are many changes to state. Redux also offer time-travel and single source of truth for state.

* To manage huge applications with complex state management, in a large scale application, Redux is a better way to control state.

* In a large scale application, Redux is a better way to control state.


2. What is the purpose of a reducer?

***The reducer takes a state and an action and returns a new state***

3. What does an action contain?

***Object literals that tell the reducer what is being done to the app, and any data required for the update.***

4. Why do we need to copy the state in a reducer?

***Reducers are not allowed to modify the existing state, instead they must make immutable updates by copying the existing state and making changes to the copied values.***

## Document the following Vocabulary Terms

* **immutable state:** This allows the state to only change when absolutely necessary to make React apps perform as well as possible.

* **time travel in redux:** This is a feature of redux dev tools that allows you to see every state that a page has been in.

* **action creator:** Actions send data from your application to your store, and are the only source of information for the store. An action creator is a function that creates an action.

* **reducer:** Reducers tell the application how to change state in response to an action.

* **dispatch:** This is the name of the function you use to send actions to the store.


## Preparation Materials

* Reducers are a great concept in Redux, because they allow your react application to have specific pieces of data that all update synchronously. All reducers run against your Redux store, and then the store triggers a change event and your entire React.js application re-renders.

* The most common state shape for a Redux app is a plain Javascript object containing “slices” of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have “slice reducer” functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

* There are two ways to define the initial shape and contents of your store’s state. First, the createStore function can take preloadedState as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser’s localStorage. The other way is for the root reducer to return the initial state value when the state argument is undefined. These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using combineReducers.

* combineReducers takes an object full of slice reducer functions, and creates a function that outputs a corresponding state object with the same keys. This means that if no preloaded state is provided to createStore, the naming of the keys in the input slice reducer object will define the naming of the keys in the output state object. The correlation between these names is not always apparent, especially when using ES6 features such as default module exports and object literal shorthands.