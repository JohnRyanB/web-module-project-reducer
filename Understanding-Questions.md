# Understanding Questions:

1. What are the steps of execution from the pressing of the 1 button to the rendering of our updated value? List what part of the code excutes for each step.

- The user presses the 1 button.
- The button runs our event handler handleChanges, which accepts the event as the paramater
  *handleChanges dispatches our addOne action in actions/index.js, passing in e.target.value(the value of the button) as a paramater.
  *the addOne action in actions/index.js passes into reducer in /reducers/index.js case "ADD_ONE", returning spread state with the pair value total, taking the total in state and adding 1.
  \*that state is then passed back to App.js as passed into the TotalDisplay component as props through its value (value={state.total})
  ...

- TotalDisplay shows the total plus 1.
