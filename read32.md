# Review

**When you have multiple contexts, what component type should you use (class/function) and why?**
can use both, but function is better

**What are some good use cases for using the Context API for global state?**  
cover image
theme  
any data need to pass to many level of compnonets

**How can you best test context?**

using behavioral testing

&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| context   |  the circumstances that form the setting for an event, statement, or idea, and in terms of which it can be fully understood.          |
| useContext()   |    hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.         |
| static context  |   block belongs to the class and these will be loaded into the memory along with the class.           |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- context

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- context with functions

_What are you most excited about trying to implement or see how it works?_

- globally passing in general

&nbsp;

&nbsp;

## Preparation Materials

> context api

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.
- Context is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.
- If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.
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
However, the management of that state (adding, removing) needs to be globally accessible.

- Higher Level API
This function uses the local state mutator useState to properly append a new alert without destroying existing ones.

- what Redux does with useContext and useReducer. The combination of these two hooks means we can have a global state and use Redux-like reducers, actions, and dispatchers to mutate that global state. To an extent, it’s possible.

&nbsp;
