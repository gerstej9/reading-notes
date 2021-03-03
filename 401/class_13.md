# Code 401 Class 13 Reading Notes

## What does it mean that web sockets are bidirectional? Why is this useful?
* Web sockets are bidirectional because they are able to listen for events from their connections as well as emit events to them. This is useful because it allows greater interactivity between the sockets and the server and it also allows sockets to interact with other sockets through the server so to speak.

## Does socket.io use HTTP? Why?
* socket.io does use http, the server side mounts onto the Node.js HTTP server and client side access the server through HTTPS
* [Source socket.io](https://socket.io/get-started/chat/)

## What happens when a client emits an event?
* When a client emits an event, that event will be sent to the server at which point the server can choose to do something such as emit a new signal or perform a function

## What happens when a server emits an event?
* When a server emits an event it will be emitted to all socket connections unless specified otherwise. This will allow client side sockets to react to the event if desired.

## What happens if a client “misses” an event?
* If a client misses an event the event will simply be ignored. The client will receive the message but choose to do nothing with it
* [Source Stack Overflow](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)

## How can we mitigate this?
* We can mititgate this issue by always having handlers but only adding logic to the handler during a state change or if desired. In this way the socket will always pick up the message.
* [Source Stack Overflow](https://stackoverflow.com/questions/32816290/what-happens-with-unhandled-socket-io-events)

## Define the following terms
* Socket
  * "A socket is end point of two way communication between two programs that are running on a network"
  * [Source Oracle](https://www.google.com/search?q=code+socket+definition&rlz=1C5CHFA_enUS917US917&oq=code+socket+definition&aqs=chrome..69i57.3314j0j4&sourceid=chrome&ie=UTF-8)
* Web Socket
  * Web socket is a protocol that enables bidirectional communication between a client and server that begins with a three way handshake and uses TCP
* Socket.io
  * Socket.io is a library in javascript that allows for bidirectional and event based communication in a way similar to Web socket protocol
  * [Source](https://socket.io/docs/v3/index.html)
* Client
  * A client refers to a program that is seperate from the server and wishing to interact with the server
* Server
  * A server is a program that is running and able to be connected to by various clients. it is the main hub so to speak
* OSI Model
  * Open System Interconnection is a reference model of how information moves from a software application in one computer to that in another
  * [Source javatpoint](https://www.javatpoint.com/osi-model)
* TCP Model
  * The Transmission Control Protocol is a modified form of the OSI model and specifies how data should be packaged, sent, and received.
  * [Source Wikipedia](https://en.wikipedia.org/wiki/Internet_protocol_suite)
* TCP
  * TCP is a connection oriented-protocol where a connection must be established between the sender and receiver.
  * [Source Private Internet Access](https://www.privateinternetaccess.com/blog/tcp-vs-udp-understanding-the-difference/)
* UDP
  * Unlike TCP, UDP is a connectionless protocol where the sender and receiver do not need to establish a connection before sending data.
  * [Source Private Internet Access](https://www.privateinternetaccess.com/blog/tcp-vs-udp-understanding-the-difference/)

[Table of Contents](README.md)