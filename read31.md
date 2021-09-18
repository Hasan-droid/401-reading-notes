# Review  

**Describe use cases useState() vs useReducer()**  
useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.  

**Why do custom hooks need the use prefix?**  
We can decide what it takes as arguments, and what, if anything, it should return. In other words, it's just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

**What do custom hooks usually do?**
Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.  

**Using any list of custom hooks, research and name one that you think will be useful in your applications**.

**Describe how a hook that fetches API data might work**.

1. Holding that data that is to be rendered
2. Page count to make API call.
3. Loading state (show loading screen/component until the data is received from server)
4. Error state (show error message when something goes wrong while fetching data)

&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| reducer  | a pure function that takes the previous state and an action, and returns the next state, used to manage state in an application         |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- costum hooks

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- costum hooks

_What are you most excited about trying to implement or see how it works?_

- hooks is a nice tools although i still not good in implement them yet

&nbsp;

&nbsp;

## Preparation Materials

> context api

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
- Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.
- If you only want to avoid passing some props through many levels, component composition is often a simpler solution than contex
- React.createContext
Creates a Context object. When React renders a component that subscribes to this Context object it will read the current context value from the closest matching Provider above it in the tree.

```React
const MyContext = React.createContext(defaultValue);
```

- Context.Provider

```React
<MyContext.Provider value={/* some value */}> 
```

- Class.contextType
Using this property lets you consume the nearest current value of that Context type using this.context. You can reference this in any of the lifecycle methods including the render function.

- Context.Consumer
A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component.

- Context.displayName
Context object accepts a displayName string property. React DevTools uses this string to determine what to display for the context.

&nbsp;

&nbsp;

> hooks and context example

- Globally Accessible
The state can be localized to a single centralized component. That same centralized component can be responsible for rendering them.
However, the management of that state (adding, removing) needs to be globally accessible

- Higher Level API
This function uses the local state mutator useState to properly append a new alert without destroying existing ones.

- what Redux does with useContext and useReducer. The combination of these two hooks means we can have a global state and use Redux-like reducers, actions, and dispatchers to mutate that global state. To an extent, it’s possibl

&nbsp;

&nbsp;
