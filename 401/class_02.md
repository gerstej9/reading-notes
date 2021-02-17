# Code Fellows 401 Class 02 Notes

## What is the difference between PUT and PATCH in regards as HTTP methods
* Simplistically PUT requires the overwriting/updating of an entire entity whereas PATCH allows for updating of partial segments.
* Both PUT and PATCH are methods for updating data.
* PUT will update and overwrite data for instance if you have an object with three properties and use a PUT to update only one it will wipe the other two. Likewise if you used a PUT with the one property on a new object that object would now have the one property.
* PATCH on the other hand allows you to modify, in the example above, the one property specified while leaving the other two properties untouched. In that sense PATCH is more delicate the PUT
* [Source: Rapid API](https://rapidapi.com/blog/put-vs-patch/)

## Resources for Mocking an API
* There are various reasons why a developer might want to avoid external APIs during a development phase. For these reasons there are resources available that allow you to "mock" an API for development and testing. Below are three resources that can be used for API mocking.
* Mirage JS available through npm
* Jest available through npm
* Cypress
* [Source: Valentino Gagliardi](https://www.valentinog.com/blog/fake/)

## Compare and Contrast Swagger and apiDoc.js
* Both apiDoc and swagger focus on documentation of api's 
* According to the apiDoc homepage, "apiDoc creates a documentation from API annotations in your source code"
* Swagger, according to their own homepage, "takes the manual work out of API documentation, with a range of generating visualizing, and maintaining API Docs"
* Both Swagger and apiDoc use json schema for operation
* apiDoc allows for inline documentation
* Swagger allows design of api structure which allows machines to work with your api easier
* Sources
* [Dev.to](https://dev.to/themsiqueira/document-a-api-nodejs-with-apidoc-69k)
* [Swagger](https://swagger.io/)
* [apiDoc.js](https://apidocjs.com/)


## Compare and Contrast SOAP and ReST
* SOAP stands for Simple Object Access Protocol and is a protocol
* REST stands for Representational State Transfer and is an architecture
* SOAP takes more bandwidth and works only with XML formats
* REST does not need as much bandwidth and is more flexible, it is also able to use SOAP but not vice versa
* REST is considered a "Restful" service in that it can use GET, POST, PUT, and DELETE
* Both have their advantages and disadvantages for instance REST is beneficial in stateless environments, when caching is not needed in great amounts and when bandwidth is limited
* SOPA is beneficial for asynchronous processing and stateful operations
* [Source: Guru99](https://www.guru99.com/comparison-between-web-services.html)


## Define the following Terms
* Web Server
  * A web server is comprised of both hardware and software, a computer that stores the software and website's files and an HTTP server in the form of software, which understands URLs and HTTP
* Express
  * Express is a Node web framework that provides the ability to write handlers for requests with HTTP verbs, it is able to intergrate view rendering agents for templating and allows for addition of middleware.
* Routing
  * Routing has to do with the determination of how a certain application will respond to a client request in terms of pointing to a specific path and depends on which HTTP method is used.
* WRRC
  * WRRC stands for Web Request Response Cycle
  * The request response cycle has to do with a client building a request for information that a server receives and then sends a response baack to the client.
* Sources
* [MDN Webdocs Web Server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server)
* [MDN Webdocs Express/Node Introduction](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)
* [Express.js](http://expressjs.com/en/starter/basic-routing.html)
* [Turing.io](https://backend.turing.io/module2/lessons/how_the_web_works_http)



[Table of Contents](README.md)