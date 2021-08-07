# Component Based UI

## Review, Research, and Discussion


**Name 5 Javascript Frameworks (other than React)**

1. Vue
2. Angular
3. Ember
4. Backbone.js
5. Svelte

**What's the difference between a framework and a library?**  
A library offers pieces that you can add to your code where you need it. A framework is in charge of the code, and you plug in your sections of the code within a framework.

### Vocabulary

| Term      | Definition                                                                            |
| --------- | ------------------------------------------------------------------------------------- |
| Rendering | This is what happens when an element is attached to the page or to the DOM.           |
| Templates | Templates allow you to break down HTML into smaller bits that can be reused.          |
| State     | State is a built-in object in React. When the state changes, the component rerenders. |


 ### What Is React?
React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called `components.`

### what is JSX?
JSX stands for JavaScript XML. It is simply a syntax extension of JavaScript. It allows us to directly write HTML in React (within JavaScript code). It is easy to create a template using JSX in React, but it is not a simple template language instead it comes with the full power of JavaScript.

### Rendering Elements:
Rendering an Element into the DOM:

![ Rendering Elements](https://user-images.githubusercontent.com/79833733/128561754-ef251c3a-ca4e-410f-ad25-65a1dc652565.png)

- Let’s say there is a `< div> `somewhere in your HTML file,We call this a `root` DOM node because everything inside it will be managed by React DOM. Applications built with just React usually have a single root DOM node. If you are integrating React into an existing app, you may have as many isolated root DOM nodes as you like.

- To render a React element into a root DOM node, pass both to ReactDOM.render():
![](https://user-images.githubusercontent.com/79833733/128562327-1d7b6062-7d3a-4074-bd64-0f581d1b6722.png)


### Updating the Rendered Element:

- React elements are immutable. Once you create an element, you can’t change its children or attributes. An element is like a single frame in a movie: it represents the UI at a certain point in time.
With our knowledge so far, the only way to update the UI is to create a new element, and pass it to ReactDOM.render().


- It calls ReactDOM.render() every second from a setInterval() callback.
React Only Updates What’s Necessary:

- React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.