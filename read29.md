
# Review

**How can we ensure that an effect hook runs only once?**

pass [] on it

**Can useState() update more than one state variable at the same time?**  

no

**Is useState() synchronous?**

yeah sure  

&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| State Hook  |  Returns a stateful value, and a function to update it.          |
| Component Lifecycle   |  Initialization > Mounting > Update > Unmount          |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- hooks

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- hooks

_What are you most excited about trying to implement or see how it works?_

- hooks again

&nbsp;

&nbsp;

## Preparation Materials

> useReducer hook

- An alternative to useState.

```React
const [state, dispatch] = useReducer(reducer, initialArg, init);
```

- Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

- useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

- There are two different ways to initialize useReducer state. You may choose either one depending on the use case.

- The simplest way is to pass the initial state as a second argument:

```React
  const [state, dispatch] = useReducer(
    reducer,
    {count: initialCount}
  );
```

- You can also create the initial state lazily. To do this, you can pass an init function as the third argument. The initial state will be set to init(initialArg).

- If you return the same value from a Reducer Hook as the current state, React will bail out without rendering the children or firing effects.

&nbsp;

&nbsp;

> Ultimate Guide to useReducer

- useReducer is used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.

- There are three main building blocks in Redux:

1. A store — an immutable object that holds the applications state data
2. A reducer — a function that returns some state data, triggered by an action type
3. An action — an object that tells the reducer how to change the state. It must contain a type property, and it can contain an optional payload property

- useState vs. useReducer
 Although useState is a Basic Hook for managing simple state transformation and useReducer is an Additional Hook for managing more complex state logic, it is worth noting that useState uses the useReducer internally. This implies that you could use useReducer for everything you can do with useState.

- When to use the useReducer Hook
Once your application grows in size, you’ll most likely deal with more complex state transitions. At this point, you will be better off using useReducer as it gives us more predictable state transitions than useState. This becomes more important when state changes become so complex that you want to have one place to manage state.
