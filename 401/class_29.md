# Code 401 Class 29 Reading Notes


## Do child components have direct access to props/state from the parent
* Child components do have direct access to parent props/state. They can access any parent functions or state that are passed down to them.

## When a component "wraps" another component, how does the child component's output get rendered
* The output from the lowest child component will return it's output to the higher level component which will then output to another parent component.

## Can a component that is a child be used as a standalone component somewhere else in an app
* Yes as long as it is provided it's necessary inputs it can be utilized as a standalone componet

## What trick can a parent use to share all props with all it's children
* ```React.cloneElement(this.props.children)```
* [Source StackOverflow](https://stackoverflow.com/questions/32370994/how-to-pass-props-to-this-props-children)

## Define the following terms
* props.children
  * this.props.children refers to a child node or an array of node children from a react component
  *[Source Learn Co](https://learn.co/lessons/react-this-props-children)
* composition 
  * composition is the "ingredients and arrangement of ingredients" in other words its all the components and how the components are arranged and layered to create a final product
  * [Sourcec RW Eruch](https://www.robinwieruch.de/react-component-composition)

[Table of Contents](README.md)