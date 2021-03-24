# Code 401 Class 27 Reading Notes

## does a deployed React application require a server?
* Node is not needed to run React because React is a client side library. The server used in development is used for the reloading of the app in response to file changes in real time.
* [Source Stack Overflow](https://stackoverflow.com/questions/60011485/why-does-react-have-a-server-on-its-own)

## Why do we prefer to test a React application at the behavior rather than the unit level
* Behavior testing provides a middle level of testing written by the developer that is based on the behavior as opposed to strictly based on code. Unit based tests are less focused on the mechanics of the code.
* [Source CodeBurst](https://codeburst.io/component-tests-vs-unit-tests-tdd-71b921d48907#:~:text=Component%20tests%20provide%20an%20intermediate,of%20the%20code%20under%20test.)

## What does npm run build do?
* Build combines all css files into one and same for javascript files creating a script that runs your application

## Describe the actual composition/ architecture of a React application
* A react application is composed of a index.js or root file that pulls from an App.js file. The app.js itself pulls from different component files that ultimately will make up the html, css and javascript of the end application.

## Define the following terms

* BDD
  * Behavior Driven Development is a form of development that is based on aiming for desired behaviors of an application or software. Utilizing the end behavior desired development is guided until the goal is reached.

* Acceptance Tests
  * Acceptance tests are tests that an application or software must pass to ensure proper functionality.

* mounting
  * Mounting is when react components are actually created and inserted onto the dom, essentially the actual rendering onto the page.
  * [Source Free Code Camp](https://www.freecodecamp.org/news/how-to-understand-a-components-lifecycle-methods-in-reactjs-e1a609840630/)

* build
  * Build in React js refers to the process and end result of turning source code into a compilation of bode that can be utilized by the browser

[Table of Contents](README.md)