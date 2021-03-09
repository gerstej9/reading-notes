# Code 401 Class 16 Reading Notes

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
* 


[Table of Contents](README.md)