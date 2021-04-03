# Code 401 Class 34 Reading Notes

## Why is the Context API useful
* Context API allows components to be able to share data without being directly connected with each other.
* [Source Blog Bit SRC](https://blog.bitsrc.io/why-you-should-consider-the-new-context-api-in-react-a-deep-dive-d588b66c57b5#:~:text=Context%20API%20is%20a%20way,the%20React%20component%20sub%2Dtree.)

## Can a component outside of a provider get its context?
* A component can access context by using the useContext hook

## What are some common use cases for using the Context API?
* Context API can be useful for themes, authorization and multilingual applications
* [Source Blog Bit SRC](https://blog.bitsrc.io/why-you-should-consider-the-new-context-api-in-react-a-deep-dive-d588b66c57b5#:~:text=Context%20API%20is%20a%20way,the%20React%20component%20sub%2Dtree.)

## Describe "Context Hell"
* Context hell is when react applications are wrapped by many contexts.
* [Source Charles Stover Medium](https://charles-stover.medium.com/you-may-not-need-a-global-god-state-in-react-206930033895#:~:text=When%20using%20the%20context%20API,contexts%20wrapping%20your%20React%20application.&text=Your%20application%20can%20be%20easier,problems%20you%20do%20not%20have.)

# Define the following terms
* Global state
  * Global state is a state that is able to be shared across all components
* Global Context
  * Global context allows for the shared understanding of events
* Provider
  * Provider makes state and context available to other components
* Consumer
  * Comsumer consumers state and context from a provider
  

[Table of Contents](README.md)