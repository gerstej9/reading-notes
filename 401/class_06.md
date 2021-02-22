# Code 401 Class 06 Reading Notes

## Explain what a Singleton is in Computer Science
* A singleton is a design pattern in which a class is only instatiated once to provide precise access throughout an entire software
* [Source David Soni](https://medium.com/better-programming/what-is-a-singleton-2dc38ca08e92)

## Explain how the Singleton pattern can be used with Node modules, specifically with classes
* One way the singleton pattern can be used with Node modules is to create  the desired class and then a second after it calle singleton
* Create a constructor function in the singleton class to check to see if an instance of the original class has already been created, if not then the singleton class will equal a new instantiation of the original class
* The singleton class will have a getInstance function that returns a new instantiation of the orginal class
* By chaining on a getInstance function to any instatiation of the original class it will result in exact same instance of the class
* [Source Mahesh Kumawat](https://medium.com/@maheshkumawat_83392/node-js-design-patterns-singleton-pattern-series-1-1e0ab71e3edf)

## If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
* Taking a singleton approach to building a middleware system would be an effective way to create a system without redundancies
* This system would allow access to functions and classes without repetition

## Define the following terms
* Router Middleware
  * Router middleware refers to middleware files that contain routing path tables and their callback functions. These files are then imported into the server file as opposed to the code being contained within it
* Dynamic Module Loading
  * Dynamic loading is the loading of variables and functions from libraries that occurs at runtime
  * [Source Javascript.Info](https://javascript.info/modules-dynamic-imports)
*  Singleton Pattern
  * The singleton pattern is the concept of only instantiating classes once in a given system so that all files use the same class instance
  * [Source David Soni](https://medium.com/better-programming/what-is-a-singleton-2dc38ca08e92)
* CRUD -> REST Method Matches
  * PUT matches with Create and Update, POST matches with CREATE, GET matches with Read, and DELETE matches with Delete
  * [Source Stack Overflow](https://stackoverflow.com/questions/6203231/which-http-methods-match-up-to-which-crud-methods)
* Mock Testing
  * Mock testing is stubbing dependencies where HTTP calls are made. This is done to test code without making calls to an external database or API
  * [Source Stack Abuse](https://stackabuse.com/using-mocks-for-testing-in-javascript-with-jes/)


[Table of Contents](README.md)
