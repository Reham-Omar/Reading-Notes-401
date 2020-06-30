# Props and State

## Forms and Inputs
- React form elements maintain internal state. 
- The creation of a parent component , manages the state for all child components of the form and passes any necessary state down into it’s inputs through the use of props.
- Each input has an onChange event that we can handle and use to update our form-container’s state each time the user interacts with an input.

## Props
- Props are arguments passed into React components.
- Props are passed to components via HTML attributes.
- To send props into a component, use the same syntax as HTML attributes:
**Example**

Add a "brand" attribute to the Car element:

```
const myelement = <Car brand="Ford" />;
```

## One Way Data flow

- State can only be passed from parent component to a child component through the use of props. 
- This enforces the idea of one way data flow. One way data flow is a way of describing that state can only be passed down the component tree (not up). 
- If a child wants to pass some data to a parent, the parent can pass a function to the child through props and the child may invoke that function and pass it data for the parent to manage.