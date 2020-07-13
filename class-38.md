# Asynchronous Actions

- Every time an action was dispatched, the state was updated immediately.
- When you call an asynchronous API, there are two crucial moments in time: 
 *the moment you start the call*, and *the moment when you receive an answer* .

- Each of these two moments usually require a change in the application state; to do that, you need to dispatch normal actions that will be processed by reducers synchronously.
- Usually, for any API request you'll want to dispatch at least three different kinds of actions:

1. An action informing the reducers that the request began.

The reducers may handle this action by toggling an isFetching flag in the state. This way the UI knows it's time to show a spinner.

2. An action informing the reducers that the request finished successfully.

The reducers may handle this action by merging the new data into the state they manage and resetting isFetching. The UI would hide the spinner, and display the fetched data.

3. An action informing the reducers that the request failed.

The reducers may handle this action by resetting isFetching. Additionally, some reducers may want to store the error message so the UI can display it.

##  Redux middleware 

- It provides a third-party extension point between dispatching an action, and the moment it reaches the reducer.
- The most common use case for middleware is to support asynchronous actions.
- It does so by letting you dispatch async actions in addition to normal actions.
*For example, redux-thunk lets the action creators invert control by dispatching functions*.
