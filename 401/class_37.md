# Code 401 Class 37 Reading Notes

## Why choose Redux instead of Context API
Context API will trigger a re-render on every component with each update of state whereas Redux will only re-render the updated components
[Source Code House Group](https://www.codehousegroup.com/insight-and-inspiration/tech-stream/using-redux-and-context-api#:~:text=Context%20API%20prompts%20a%20re,a%20log%20in%20each%20component.)

## What is the purpose of a reducer
* A reducer takes in an initial state, an action and a payload and performs an action that results in a change in state.

## What does an action contain
An action contains a case, logic to be performed in that case and returns a new state

## Why do we need to copy the state in a reducer
* If new state is different from the initial state the "reducer must create a new copy" as a way to describe the unchanged part.
* [Source Stack Overflow](https://stackoverflow.com/questions/39521868/why-does-redux-need-to-make-a-copy-of-the-data-each-time-it-changes#:~:text=The%20only%20way%20to%20change,dispatch%20should%20be%20used%20instead.&text=If%20the%20new%20state%20is,to%20describe%20the%20unchanged%20part.)

## Define the following terms
* Immutable State
  * Is a state that cannot be changed
* Time travel in redux
  * Is part of the redux dev tools that allows state changes to be reversed
  * [Source Medium](https://medium.com/the-web-tub/time-travel-in-react-redux-apps-using-the-redux-devtools-5e94eba5e7c0)
* Action creator
  * "An action creator is a function that returns an action object". It consists of a utility function and action creators.
  * [Source Redux Book](https://read.reduxbook.com/markdown/part1/04-action-creators.html)
* Reducer
  * A reducer is a function that is part of redux and is capable of creating a state change and initiating a re-render
* Dispatch
  * Dispatch is a function within redux that causes a state change. With Redux, using the connect function utilizes dispatch for you
  * [Source react-redux.org](https://react-redux.js.org/using-react-redux/connect-mapdispatch)


[Table of Contents](README.md)