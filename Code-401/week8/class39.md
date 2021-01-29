# Code 401 | Redux - Additional Topics

## Class 39 Reading Notes

I. Research Questions

- What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?: I believe that the answer to this question lies in doing a get call in a useEffect on a high-level component.

- When using a thunk/async action that dispatches the actual action, which do you export from your reducer? The async action is exported, not the actual action.

II. Vocabulary

- Middleware: "software that acts as a bridge between an operating system or database and applications, especially on a network" (Oxford).

- Thunk: a library in React's Redux library that allows for async API calls.

III. Reading Links

- [Redux Toolkit](https://redux-toolkit.js.org/)
- ["Intermediate Tutorial: Redux Toolkit in Action"](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)
- [Alternative State Manager: MobX](https://mobx.js.org/getting-started.html)
- [Alternative State Manager: Hookstate](https://mobx.js.org/getting-started.html)
- []

IV. Preview Questions

A. Which 3 things had you heard about previously and now have better clarity on?

- Thunk
- Redux toolkit
- Alternative state managers

B. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Redux toolkit
- Thunk
- Alternative state managers

C. What are you most excited about trying to implement or see how it works?: Rendering start-up state from API.

[<--back](401week8.md)

[<--home-->](../../README.md)
