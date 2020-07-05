# Custom Hooks

## What is Custom Hooks?
- Custom Hooks are a mechanism to reuse stateful logic (such as setting up a subscription and remembering the current value), but every time you use a custom Hook, all state and effects inside of it are fully isolated. 

## How does a custom Hook get isolated state? 
- Each call to a Hook gets isolated state.

## What is the purpose of a custom hook?
- The Effect(useEffect) hook allows you to perform side effects in a functional component, think of it like lifecycle events in class components.
- A custom hook is a function that starts with the word “use” and may call other hooks

##  Common use cases – make things DRY!
- Handle forms easily
- Pre-fetch API data
- Connect to services (like socket.io, Q, etc)