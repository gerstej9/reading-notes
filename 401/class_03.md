# Code 401 Class 03 Reading Notes

## Real World Uses for Middleware
* Middleware can be used effectively for error-handling
* Middleware can also be used for request validation
* Lastly middleware can be used for logging certain information such as the path, method, and time of each request

## True or false: The route handler is middleware
* Route handlers are not middleware by definition they are handler functions. When there is one callback function this holds true, however, middleware functions can be inserted into the route handler function

## In what ways can a middleware function end the process and send data to the browser?
* Middleware functions can use a response. to send information back to the client side or they can use a next() which will then kick back to the following server operation

## At what point in the request lifecycle can you inject middleware?
* Middleware can be injected after the request has been made and before the response has been sent.
* For instance middleware error handlers can be injected if there is a request for a falty path

## What can cause express to error with "Request header sent twice, cannot start a second response"
* Calling next() twice or any response. after another has already been sent within a function or callback will result in this error

## Define the following terms
* Middleware
  * Middleware refers to code that is imported into the server that can be used in between the request and response of a server
* Request Object
  * Is the information sent from the client to the server including the path and http method
* Response Object
  * The response object is the information sent from the server to the client and can be a redirect, json object, file download or various other actions
* Application middleware
  * Application middleware is software that operates in between the request and response cycle that plays a role in the function of the application such as database middleware
* Routing middleware
  * Routing middleware is software that operates between the request and response cycle that plays a role in path routing such as error handling middleware
* Test Driven Development
  * Test driven development is an aspect of AGILE develoment and operates on the principle of testing code as it is developed. This process takes slightly longer in the development phase but that is greatly offset by the reduction in time needed for fixing bugs. In addition it allows for continuous intergration and continuous development/deployment.
* Behavior testing
  * Behavior testing is another aspect of AGILE that specificies testing of units of software be driven by the desired behavior of the unit.

## Sources
* [Stack Overflow Middlware](https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres#:~:text=They%20are%20not%20middleware%20functions,the%20only%20one%20callback%20function.)
* [TutorialsPoint Express Middleware](https://www.tutorialspoint.com/expressjs/expressjs_middleware.htm)
* [Stack Overflow Request Headers](https://stackoverflow.com/questions/7042340/error-cant-set-headers-after-they-are-sent-to-the-client)
* [Cake PHP Request and Response Objects](https://book.cakephp.org/3/en/controllers/request-response.html#:~:text=The%20request%20and%20response%20objects,HTTP%20responses%20from%20your%20controllers.)
* [Wikipedia Middleware Definition](https://en.wikipedia.org/wiki/Middleware#:~:text=Middleware%20is%20computer%20software%20that,available%20from%20the%20operating%20system.&text=Middleware%20makes%20it%20easier%20for,specific%20purpose%20of%20their%20application.)
* [Wikipedia Behavior Driven Development](https://en.wikipedia.org/wiki/Behavior-driven_development)


[Table of Contents](README.md)