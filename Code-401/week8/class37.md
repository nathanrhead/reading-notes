# Code 401 | Redux - Combined Reducers

## Class 37 Reading Notes

I. Research Questions

- Why choose Redux instead of the Context API for global state?: because full state from each reducer is accessible to any and all components that need it. Though there seems to be an ongoing debate about the benefits and drawbacks of redux vs context.

- What is the purpose of a reducer?: "A reducer is a function that determines changes to an application's state. It uses the action it receives to determine this change" ([CSS-ticks.com](https://css-tricks.com/understanding-how-reducers-are-used-in-redux/#:~:text=A%20reducer%20is%20a%20function,so%20that%20they%20behave%20consistently.)).

- What does an action contain?: a type of action and a payload.

- Why do we need to copy the state in a reducer?: The copy is a way of determining which part of state has changed and which has stayed the same. In addition, state is by designed in redux to be immutable, thus requiring a copy.

II. Vocabulary

- immutable state: the concept that the initial state ought not be changed, only modified in a copy, in order to centralize mutations, allowing for easier debugging, to simplify the code and make it more readable and predictable, and to optimize performance.

- time travel in redux: "The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app" (["Time Travel in React Redux apps using the Redux DevTools](https://medium.com/the-web-tub/time-travel-in-react-redux-apps-using-the-redux-devtools-5e94eba5e7c0#:~:text=The%20Redux%20DevTools%20records%20dispatched,page%20or%20restarting%20the%20app.)).

- action creator: a function that returns an action object.

- reducer: a function that determines changes to state.

- dispatch: the redux method that dispatches actions to reducers that trigger changes to state.

III. Preview Links

- ["Multiple Reducers with Redux Reducers - Redux React Tutorial #4" Video](https://www.youtube.com/watch?v=gBER4Or86hE)
- ["Using combineReducers"](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)
- ["combineReducers(reducers)"](https://redux.js.org/api/combinereducers/)

IV. Preview Questions

A. Which 3 things had you heard about previously and now have better clarity on?

- Combining reducers.
- The reasons initial state is meant never to be changed.
- Redux vs context.

B. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

- .dispatch()
- Time travel.
- Action creators.

C. What are you most excited about trying to implement or see in action?: useReducer() and time travel.

[<--back](401week8.md)

[<--home-->](../../README.md)
