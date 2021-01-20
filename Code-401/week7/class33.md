# Code 401 | Context API

## Class 33 Reading Notes

I. Research Questions

- Describe use cases for useMemo() and useReducer():
  - useMemo() memoizes a function's output. Memoizing is a method of optimizing a computer program by storing and returning the result of a costly function, instead of the function itself.
  - useReducer(): "It accepts a reducer function with the application initial state, returns the current application state, then dispatches a function" (css-tricks.com).

- Why do custom hooks need the "use" prefix?: convention, I think. According to the docs, "Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it."

- What do custom hooks usually do?: They're used to provide the logic needed for two or more functions in a reusable manner.

- Using any list of custom hooks, research and name one that you think will be useful in your applications:
  - npm i react-use-form-state
  - npm i react-fetch-hook (is there one for Axios?)

- Describe how a hook that fetches API data might work: like a router, you can store all of the logic for your calls in a hook and implement that hook whenever you want to make an API call. Would boilerplate calls work for various APIs?

II. Vocabulary:

- Reducer: "A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change. We have tools, like Redux, that help manage an application's state changes in a single store so that they behave consistently. . . . Redux relies heavily on reducer functions that take the previous state and an action in order to execute the next state" [CSS-tricks.com](https://www.google.com/search?q=what+is+a+reducer+in+react%3F&oq=what+is+a+reducer+in+react%3F&aqs=chrome..69i57j0i22i30i457j0i10i22i30j0i22i30.8414j1j7&sourceid=chrome&ie=UTF-8).

III. Preview Links

- ["Context"](https://reactjs.org/docs/context.html)
- ["Snackbars in React: An Exercise in Hooks and Context"](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
- [awesome-react-context github repo](https://github.com/diegohaz/awesome-react-context)

IV. Questions to Guide Reading

A. Which 3 things had you heard about previously and now have better clarity on?

- Memoization
- Hooks
- Context

B. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Context
- useReducer()
- How to pass "props" without passing "props"? Or, rather, is it okay to use hooks AND pass props when convenient?

C. What are you most excited about trying to implement or see how it works?: context.

[<--back](401week7.md)

[<--home-->](../../README.md)
