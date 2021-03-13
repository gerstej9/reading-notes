# Code 401 Class 19 Reading Notes

## What is the difference between a FIFO and standard queue
* A FIFO queues have similar features to standard queues but also are able to perform exactly-once proccessing or in other words making sure they read/write only one exact time. FIFO queues help to stop unintentional duplicates.
* [Source Amazon AWS](https://aws.amazon.com/about-aws/whats-new/2016/11/amazon-sqs-introduces-fifo-queues-with-exactly-once-processing-and-lower-prices-for-standard-queues/#:~:text=FIFO%20queues%20have%20essentially%20the,being%20received%20by%20message%20consumers.)

## How can a server be assured a message was properly received?
* A server can expect a response from a client to prove as a confirmation that a message was properly received, as a fail safe it can keep it in a queue until the confirmation is received.

## What classic design pattern is best represented by event driven programming
* An observer pattern is represented by event driven programming because it consists of an object maintaining observers that are looking for state changes a.k.a events.

## How do you test an event driven system
* To test an event driven system you can start with unit tests where you test the individual functions and components of each part of the system. You can also test connections to make sure everything is interconnected as expected. Last you can perform end to end tests simulating actual event changes and monitoring output.
* [Source Dan Siwiec on Medium](https://medium.com/dan-on-coding/testing-event-driven-systems-63c6b0c57517)

## Define the following terms
* Serverless API
  * A serverless API is based on a cloud service that allows for the creation of API endpoints with specific http request methods such as POST and GET. This allows a coder to create a website without needing a server to host their code.
* Triggers
  * Triggers are a way of setting up functions to activate based on certain events. When an event occurrs, a trigger initiates a specific function as a result.
* Dynamo vs. Mongo
  * Dynamo and Mongo are both NoSQL databases, Mongo is independent while Dynamo is an AWS service.
* Dynamoose vs. Mongoose
  * Dynamoose and Mongoose are npm packages that allow for node.js interface with DynamoDB and MongoDB respectively


[Table of Contents](README.md)