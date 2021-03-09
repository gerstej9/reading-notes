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
* Server Instances
  * Server instances refer to an instance of server deployment. For instance on AWS an instance can be created on a virtual machine that is hosting a server and then that instance can be stopped.
* Containers
  * Containers are services that package software into units for development, shipment and deployment and can be used to hold files and other software used in online applications
  * [Source Docker](https://www.docker.com/resources/what-container)
* Cloud Services 
  * Cloud services refer to virtual machine services that are accessible through the internet. These services can be storage, web hosting, and other forms of computer activities that one uses an online computer for. Examples are AWS and Azure
* Cloud Architecture
  * Cloud architecture refers to the components that are necessary for building a cloud and consist of a front-end, back-end, cloud based delivery, and ndetwork.
  * [Source vmWare](https://www.vmware.com/topics/glossary/å)

* AWS
  * AWS is Amazon Web Services and refers to Amazon's cloud computing services. They offer various services that range from S3 storage containers to Elastic Beanstalk which is able to host web applications
* EC2/Beanstalk vs. Heroku
  * EC2 refers to the elastic computing service and beanstalk is a way to deploy applications in a way similar to Heroku. These two solutions offer roughly comparable services, SQL services on AWS are more secure, and Herokue offers more robust Dynos. At the same time Heroku is easier to use and setup but has greater price jumps with scaling.
  * [Source John Tucker, CodeBurst](https://codeburst.io/heroku-v-s-aws-elastic-beanstalk-1cc6f12ca3c7)

[Table of Contents](README.md)