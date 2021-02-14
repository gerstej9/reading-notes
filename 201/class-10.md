# Class 10 Notes

## JavaScript Chapter 10: Errors and Debugging
* When troubleshooting it is important to consider order of execution of code
* It is also important to understand execution context such as global or within a function
* The JavaScript interpreter processes one line of code at a time, when a statement needs data from another function it stacks the new function on top of the current task
* Each time a script enters a new execution context there are two phases of activity
    1. Prepare: The new scope is created and variables, functions, and arguments are created
    2. Execute: Assign values to variables, reference functions and run their code and execute statements
* Each execution context has its own variables object that holds variables, functions and parameters within it, it can also access its parents variables object
* In JS if a statement generates an error then it throws an exception and at that point the interpreter stops and looks for exception-handling code
* Error objects can help you find where your mistakes are and browsers have tools to help you read them
    * Some examples include syntax, reference, eval, URI, type, generic, range and NaN

## How to Deal with Errors
* Debug the script to fix errors and handle errors gracefully
* Debugging workflow involves deduction and process of elimination
* Browser dev tools and javascript console will help tell you where the problem is and what it is
* You can log data to the console using the console.log function
* console.info, .warn, and .error are also helpful as is console.group for grouping messages
* In certain browsers console.table method allows you to output a table of information including objects and arrays
* Using console.assert() you can test if a condition is met
* Breakpoints in debugging tools allow you to stop at a certain line of code
* Once stopped using a break point you can step trhough lines one by one, step into a function or step out of a function
* In some browsers you can set conditional breakpoints using a pop up box and a condition
* The "debugger" keyword will set a breakpoint in dev tools
* Handling exceptions with try, catch, finally method
* Try code that you think might cause an exception
* Catch with a seperate set of code if exception is caused
* Finally will run either way
* If you know something might cause a problem for your script you can generate your own errors before the interpreter creates them. ```throw new Error('message');```
* Throw errors for Nan can be helpful to not effect code further down the line.
* Debugging tips
    * Another browser
    * Add numbers
    * Strip it back
    * Explaining the code
    * Search
    * Code playgrounds
    * Validation tools
* Common Errors
    * Go back to basics
    * Missed/Extra characters
    * Data type issues


[Table of Contents](README.md)