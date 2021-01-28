# Code 401 | Redux - Asynchronous Actions

## Class 38 Reading Notes

I. Research Questions

- How granular should your reducers be?: Good question. Shouldn't they do as much or as little as they need to do? I mean, no more and no less?

- Pro or Con?: multiple reducers can “fire” when a commonly named action is dispatched?: Good for less code, bad for unintended overlap.

- Name a strategy for preventing the above: Name the callbacks differently? According to the React docs, there is no default one-to-one mapping between reducers and actions. "We suggest you write independent small reducer functions that are each responsible for updates to a specific slice of state. We call this pattern “reducer composition”. A given action could be handled by all, some, or none of them. This keeps components decoupled from the actual data changes, as one action may affect different parts of the state tree, and there is no need for the component to be aware of this" (["Redux FAQ: Actions"](https://redux.js.org/faq/actions)).

II. Vocabulary

- Store: the file that combines all reducer files and makes global state available to all subscriber components.

- Combined reducers: Reducers, with their actions and payloads, copy and update state; combined in the store, they create a global or combined state that is available to all subscribers of the store.

III. Preview Links

- ["Redux Fundamentals, Part 6: Async Logic and Data Fetching"](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)
- ["Redux Thunk"](https://github.com/reduxjs/redux-thunk)
- ["Understanding Asynchronous Redux Actions with Redux Thunk"](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)

IV. Questions for the Reading

A. Which 3 things had you heard about previously and now have better clarity on?

- Combining reducers.
- The Thunk library.
- Persisting data in React.

B. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- Combining reducers.
- The Thunk library.
- Persisting data in React.

C. What are you most excited about trying to implement or see in action?: Updating redux state and a database at the same time.

[<--back](401week8.md)

[<--home-->](../../README.md)
