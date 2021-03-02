# Code 401 Class 12 Reading Notes

## What is the benefit of transforming data into packets
* Transferring data in packets is used for reliability and efficiency. If any individual packet has an issue with being sent it can be resent without affecting the entire transmission. It also potentially allow for transmission of larger amounts of data that can then be reassembled.
* [Source Tech Terms](https://techterms.com/definition/packet)

## UDP is often referred to as a connectionless protocol. Why is this?
* UDP does not establish a connection before sending data and therefore it is sometimes referred to as connectionless.
* [Source WikiBooks](https://en.wikibooks.org/wiki/Communication_Networks/TCP_and_UDP_Protocols/UDP)

## Can a socket server application have multiple socket connections?
* While a server socket listens on a single port it is able to have multiple connections on the same server as long as they are associated with different client-side IP/Port pairs.
* [Source Stack Overflow](https://stackoverflow.com/questions/11129212/tcp-can-two-different-sockets-share-a-port/11129641)

## Can a socket connection application be connected to multiple socket servers
* A single client side connection should only be used to connect to one socket server
* [Source Stack Overflow](https://stackoverflow.com/questions/5402019/connecting-to-multiple-servers-from-a-single-client-socket-c#:~:text=If%20your%20program%20is%20a,socket%20at%20all%2C%20just%20connect%20.)

## Can an application be both a socket server and a socket connection?
* You can create an application that is both a socket server and a socket connection by using UDP
* [Source Quora](https://www.quora.com/Can-you-make-a-client-socket-and-a-server-socket-in-one)

## Define the Following Terms
* Observer Pattern
  * A software design pattern where an object maintains observers and notifies them of state changes.
  * [Source Wikipedia](https://en.wikipedia.org/wiki/Observer_pattern)
* Listener
  * A listener is a function that "listens" for a specific event to occur
* Event Handler
  * An event handler is a function that is trigerred by a specific event, it is usually cued by an event listener
* Event Driven Programming
  * Event driven programming is where the flow of the application/program is driven by events usually triggered by the user
* Event Loop
  * The event loop is responsible for monitoring the call stack and pushing events from the queue to the stack when the stack is empty
* Event Queue
  * The event queue is responsible for storing functions and pushing them to the call stack when the call stack is empty. Whether or not a function is directed to the callstack or the queue initially has to do with synchronicity. It operates on a first in first out principle
* Call Stack
  * The call stack is responsible for the execution of functions and acts as a waiting line so to speak for functions. It operates on a first in last out principle
* Emit/Raise/Trigger
  * These terms correspond to aspects of event driven programming. Emit is a message sent to elicit the triggering of a response and emit raises an event. Trigger is the inititaion of a function based on a emitted/raised event.
* Subscribe
  * A subscriber is a method that sets up an event publisher
* Database
  * A database is a storage of data that can take many forms such as mongoDB, SQL, or even just arrays.

[Table of Contents](README.md)