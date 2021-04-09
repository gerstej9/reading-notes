# Code 401 Class 39 Reading Notes

## What's the best practice for "pre-loading" data into the store (on application start) in a redux application?
* The best way is to fire an asynchronous action in the lifecycle method of component will mount.
* [Source Stack Overflow](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux#:~:text=1%20Answer&text=The%20most%20'redux%2Dlike',Component%20that%20wraps%20your%20app.)

## When using a thunk/async action that dispatches the actual action, which do you export from your reducer
* You export the thunk/async action, when it is called it will perform it's async action and then invoke the actual action

## Define the following terms
* middleware
  * Middleware in general refers to software that comes inbetween two phases. In the case or redux middleware can refer to something like "thunk" where it provides the ability for a reducer to perform async functions before and is applied prior to export to the app
* thunk
  * Thunk refers to redux middleware that allows for async functions to be performed in reducers. It comes from the "past tense" of think.

[Table of Contents](README.md)