# Code 401 Class 33 Reading Notes

## Describe use cases for useMemo() and useReducer()
  *  A reducer hook is a complex version of a state hook that is used when the updated value is dependent on the previous value being change. It is also helpful when their are multiple sub-values to be changed
  * A useMemo() hook is used for memorizing a calculation function that will only recompute when one of the dependencies is changed and thereby calculation does not need to be done regularly rather the useMemo will automatically do that and save the new value
  * [Source Reactjs.Org](https://reactjs.org/docs/hooks-reference.html)

## Why do custom hooks need the use prefix?
* Custom hooks use the "use" prefix because it is a convention that allows for checking of violations of rules of hooks.
* [Source Reactjs.Org](https://reactjs.org/docs/hooks-reference.html#usereducer)

## What do custom hooks usually do?
* "Custom hooks are a way to reuse stateful logic" or in other words it allows for repeat functionality when needed
* [Source Reactjs.Org](https://reactjs.org/docs/hooks-reference.html#usereducer)

## Using any list of custom hooks, research and name one that you think will be useful in your applications
* The useArray hook looks particularly helpful beacuse array manipulation is so common in javascript
* [Source BitSRC blog](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)

## Define the following Vocabulary term
* Reducer
  * A reducer in regards to react refers to a hook that changes state using a setter when there are sub values or more complex items than useState can handle


[Table of Contents](README.md)