# Code 401 Class 18 Reading Notes

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
* Serverless Functions
  * Serverless functions can be thought of as micro-applications and micro-architecture. They are usually event triggered code and targeted code. One of the benefits is that functions can scale independently as needed.
* Cloud Storage
  * Cloud storage refers to file and data storage in the cloud or in other words on servers accessible through the internet. Examples of cloud storage are AWS S3 and iCloud by Apple.
* CDN
  * CDN refers to content delivery network. They are combinations of geographically located servers that allow for fast delivery of data. When a user accesses a cdn the servers which are located closest are activated. An example of CDN can be found in jQuery and Font Awesome
  * [Source CyberHoot](https://cyberhoot.com/cybrary/content-delivery-network-cdn/)

[Table of Contents](README.md)