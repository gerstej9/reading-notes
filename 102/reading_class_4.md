# Comparison, Logical Operators, and Loops

## Comparison Operators
* You can evaluate a situation by comparing two values and getting a boolean result
    * ```==``` equal to meaning a string 42 can equal a number 42
    * ```!=``` not equal to
    * ```===``` strict equal to meaning a string 42 must equal a string 42
    * ```!==``` strict not equal to same concept as strict equal
    * ```>``` greater than
    *  ```<``` less than
    * ```>=``` greater or equal
    * ```<=``` less than or equal

## Logical Operators
* Comparison operators return true false while logical operators allow comparison of results from more than one comparison operator
    * ```(5<2) && (2>=3)```
* ```&&``` tests more than one condition, "and" operator
* ```||``` "or" operator
* ```!``` "not" operator
    * ```!(2<1)``` returns "true"
* Logical expressions are examined left to right
    * Short circuit evaluation means the operator will stop if the answer is determined after the result is no longer possible

## Loops
* Loops check a condition and if true the code block will run. This repeats until condition returns false
* Three different types of loops
* For loops run for a specified number of times
* While loops are for an unspecifed amount of times so long as condition is true
* Do While loops similar to while but will always run the code at least once even if the condition is false
* Loops consist of keyword, condition counter, opening curley brace, code to execute during loop and closing curley brace
* ```for (var i = 0; i<10; i++){ document.write(i);}```
* A for loop uses a counter as a condition and is made up of three statements
    * Initialization ```var i =0;```
    * Condition ```i<10;```
    * Update ```i++```
* While loops operate similar to for loops but with a different structure
    * ```var i =1; var msg =''; while (i<10){msg += i{'x 5 =' +(i *5) + '<br/>; i++;}```
    * Two statements the first uses the +- operator meaning msg = msg +'newMsg' ```msg+=```
    * The second increments the counter variable by one ```i++```


[Home](README.md)