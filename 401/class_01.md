# Code 401 Class 01 Reading Notes

## Array.map()
* Array.map() is a function that allows the user to iterate over an array and perform an action on each value of the array.
* Array.map() will return an array of the resulting values of each individual array value that has been manipulated.
* For instace if you were to perform an array.map() on an arr of [1, 2, 3] in which the action performed is adding 1 to each value the return value would be [1+1, 2+1, 3+1] or in other words [2, 3, 4].
* The syntax for array is as follows ```let arr = [1, 2, 3]; arr.map(number => number +1)```
* In this example, the word number in the parentheses following arr.map is a placeholder that is used to designate an individual value of the array. What it is saying is for each "number" in the array "do this" and in this case that would be adding 1. If we had an array of cats we could use the placeholder cat in the parentheses to indicate what each individual value is.

## Array.reduce()
* Array.reduce() is a function that allows the user to start with an individual value and have accumulating effects as a result of iterating through an array.
* For instance if you had an array of numbers, you could use reduce to start at 0 and add all the numbers together to get a sum of all the values in the array.
* A user could also take an array of words and use reduce to create a single string of all the individual words in an array.
* The array.reduce function works by taking a callback function, this callback function has two parameters, an accumulator and a current value. The current value will indicate the 1st, and then 2nd and so on values of the array as it loops through. The accumulator value will be the resulting value after each iteration.
* A arr.reduce callback function will look something like this ```const reducer = (accumulator, current value => accumulator + current value```
* The arr.reduce function itself will look as follows ```arr.reduce(reducer);```
* In the case of an array of numbers ```let arr = [1, 2, 3, 4]; arr.reduce(reducer)```
* In the example above the initial current value will be 1 and the accumulator zero, on the next iteration the accumulator will be 1 and the current value 2, next 3 and 3, followed by 4 and 6 and the return value will be the final accumulation which will be 10
* Citation MDN Web Docs https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce

## Superagent()
* Superagent is a dependency that can be used in Node.js as a way to make API calls and web requests.
* Because superagent must retrieve information and therefore takes time it can be handled with a Promise or async/await functionality. 
* Code examples of this would be as follows ```superagent.get('targeturl').then(data => do something with data).catch(error => console.error(error));```
* The above example utilizes a promise wherein the superagent function will retrieve information from a target url, the .then means when the data is returned do something with it. In this case "data" is a placeholder and can be called anything. We utilize a .catch() afterwards in case an error occurs during the retrieval or manipulation of the data.
* The superagent request can also be handled with async/await functionality like so ```async function superagentRequest = () => {const data = await superagent.get('targeturl); do something with data}

## Promises
* A promise is an object that produces a value or an error at some point in the future. Promises are used for functions that take an amount of time, if that function executes succesfully it will return a value and if not it will return an error. Promises use "resolve" and "reject" as parameters and in the promise function "resolve" and "reject" are used to indicate a succesful or unsuccesful scenario much like .then() and .catch() or try{}/catch{}.


## Are all callback functions considered to be Asynchronous? Why or Why Not?
* Not all callback functions are asynchronous, a great example of this is provided above in the example for utilizing array.reduce. In that example the callback function indicates how the array should be handled but it happens at the time of and not asynchronously. Callback functions can be asynchronous, however, they are not bound to either synchronous or asynchronous.


[Table of Contents](README.md)