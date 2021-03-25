# Code 401 Class 28 Reading Notes

## Can a parent component access the state of a child component
* For a parent component to access the state of a child component the most common method used is a callback function so that the child can pass the value upwards to the parent.
* [Source Linguine Code](https://linguinecode.com/post/get-child-component-state-from-parent-component)

## What can be passed along in a prop variable
* Props stands for properties so anything that is a property of a component can be passed unidirectionaly downward to its children components.
* [Source Log Rocket](https://blog.logrocket.com/the-beginners-guide-to-mastering-react-props-3f6f01fd7099/)

## How can a child component "know" the state of another component
* If a child component uses a callback function to provide a parent component with information and then that parent component provides it to another, different, child component.

## Define the following terms
* Component props
  * Component props refers to the properties that are passed from a parent component to a child component
* Component State
  * Component state refers to the properties of the component proper
* Application State
  * Application State refers to the properties of the master application as a whole

[Table of Contents](README.md)