# Component Lifecycle / useEffect() Hook

## Review

 **1. Why do we not need more .html pages in a multi-page React app?**

In the Multipage apps , we split up our components but a lot of pages are going to be normal HTML pages, and widgets we dump in like an Image gallery that is managed by React, so the entire page is not under React control.

**2. If we wanted a component to show up on every page, where would we put it and why?**

Inside a < Route />: because React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.
**3. What does routing do with the components that were rendered when a new route is requested**

it goes to the new componetnt and remove the old one

**4. What does props.children contain?**

props.children represents the content between the opening and the closing tags when invoking/rendering a component.
can have one element, multiple elements, or none at all, its value is respectively a single child node, an array of child nodes or undefined. 

**5. How do useState() and this.setState() differ?**

setState is merging the previous state with the new one, it means that you dont have to pass the full state object every time you want to change some part of the state. React will update given properties and won’t touch the rest. The useState’s updater rewrites a previous state with a new one and it does not perform any merging. Its just replacement instead of merging

## Vocabulary Terms

**State Hook The useState()**  is a Hook that allows you to have state variables in functional components, it takes the initial state as an argument and returns an array of two entries.

**Mounting and Un-Mounting:**

**- Mounting:** is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components).

**- Un-Mounting:** This method is called just before the component gets destroyed. Any clean up statements should be executed inside this method.

### What does useEffect do?

By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

### When exactly does React clean up an effect?

React performs the cleanup when the component unmounts. However, effects run for every render and not just once. This is why React also cleans up effects from the previous render before running the effects next time.