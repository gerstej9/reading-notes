# Intro, Scripts, Expressions, Operators, and Functions

## Introduction
* Javascript allows you to;
    * Acess content within webpages
    * To modify content
    * Program rules
    * React to events
    * Some examples include slideshows, forms, reloading part of a page and filtering data
* HTML and CSS Refresher
* HTML elements consist of opening tag containing attribute name and attribute value and a closing tag
    * ```<p class ="fruit">peach</p>```
* CSS rules have a selector and declaration block which consists of property name and value
    * ```.fruit{color:pink;}```

## Scripts
* A script is a series of instructions such as a recipe or manual
* To write a script you need to state your goal and list the tasks needed to complete it
    * Define the goal
    * Design the script
    * Code each step
* Code vocabulary and syntax are paramount for writing a script
* Sketching out tasks in flowcharts fcan be helpful to see how tasks fit together

## Expressions and Operators
* An expression evaluates into results in a single value
* There are roughly two types of expressions
    * Expressions that assign a valuable to a variable
    * ```var color = 'beige' ```
    * Expressions that use two or more values to return a single value
    * ```var area = 3 * 2 ```
* Expressions rely on operators which allow programmers to create a single value from one or more values
    * Assignment operators assign a value to a variable
    * Arithmetic operators peform basic math
    * String operators combine two strings
    * Comparison operators compare two values and retun true or false
    * Logical operators combine expressions and return true or false
* Arithmetic operators allow for 
    * addition +
    * Subtraction -
    * Division /
    * Multiplication *
    * Increment ++
    * Decrement --
    * Modulus % Divides two values and returns the remainder
    * Order of operations PEMDAS
* String operators only use the + symbols for adding
* Joining of two strings together is known as concatenation
* Numbers added to strings become part of the string
* Arithmetic cannot be performed on string numbers
* An arithmetic function on a string will return NaN not a number

## Functions
* Functions let you group a series of statements together to perform a specific task
* This allows you to reuse a function in different areas without typing out all the code within it every time
* Allows for storing code if you need function to be called upon like a user click
* When you ask a function to perform you are 'calling' the function
* Functions are contained within a code block and some may need information inputted to perform which are known as parameters
* Functions deliver an answer known as a return value
* To declare a function you need a function keyword, function name and the statements that perform the task which sit in the code block
*  ```function sayHello(){document.write('Hello')}```
* To call a function you use the function name followed by parentheses and a semi-colon
* ```sayHello();```
* When defining a function that needs parameters you need to add the names in the function parentheses
    * ```function getArea(width,height)```
    * Statement ```return width*height```
    * Calling it ```getArea(3,5)```
    * Results ```15```
    *  You can also add variables into the parameters if the variables have been defined
    * Functions can be used to define other variables
    * ```wallOne = getArea(3,5)``` now wallOne = 15

[Home](README.md)


