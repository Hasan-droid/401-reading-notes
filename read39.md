# Review

**What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application??**
The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount ) of a Higher Order Component that wraps your app.

## When using a thunk/async action that dispatches the actual action,which do you export from your reducer

 the action

&nbsp;

&nbsp;

## Vocabulary

| voc | related to |
| --- | ---------- |
| middlewar | snippet of code that provides a third-party extension point between dispatching an action and the moment it reaches the reducers.           |
| thunk  |  middleware that allows you to return functions, rather than just actions, within Redux.            |
|

&nbsp;

&nbsp;

## Preview

_Which 3 things had you heard about previously and now have better clarity on?_

- Redux Toolkit (RTK)

_Which 3 things are you hoping to learn more about in the upcoming lecture/demo?_

- Redux Toolkit (RTK)

-
-

_What are you most excited about trying to implement or see how it works?_

- Redux Toolkit (RTK

&nbsp;

&nbsp;

## Preparation Materials

> Redux Toolkit (RTK)

- The Redux core library is deliberately unopinionated. It lets you decide how you want to handle everything, like store setup, what your state contains, and how you want to build your reducers.

- This is good in some cases, because it gives you flexibility, but that flexibility isn't always needed. Sometimes we just want the simplest possible way to get started, with some good default behavior out of the box.

- install by terminal
`npm install @reduxjs/toolkit react-redux`

- then use
`import { configureStore } from '@reduxjs/toolkit'`

- MobX is unopinionated and allows you to manage your application state outside of any UI framework. This makes your code decoupled, portable, and above all, easily testable.
&nbsp;
