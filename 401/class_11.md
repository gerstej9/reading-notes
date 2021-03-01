# Code 401 Class 11 Reading Notes

## Event Driven Programming in Node.js
* This describes a logical pattern that confines programming within to avoid issues during execution.
* This pattern utilizes event handlers, and a main loop that listens for event triggers
* Node.js has a built in module for event driven programming called EventEmitter
* The event emitter can be imported by requiring 'events'
* event emitter has an on method to set the listener
* It also has an emit function that is used to triggeer the event
* Removing listeners can be done with the removeListener or removeAllListeners methods
* Object Oriented Programming and Event Driven Programming can be a beneficial combination for various situations
* One example of this is to allow objects to emit events which reduces the need for one object to need to reach inside another.
[Source Digital Ocean](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)

## Why is access control important
* Access control is important because it allows for a server to host certain paths while preventing access to all users. There are instances where certain sites or capabilities should only be accessed by certain users such as administrators who need to be able to maintain aspects of the site from the client side.

## Describe an application that would need access control
* One example of an application that would need access control would be teachable, an online school platform. In the case of teachable all users can see a school's prsence but only those enrolled in the school can view the course material. Furthermore there is the course owner who can assign content creators and other administrative priviliges.

## What is a role used for
* A role is used to designate access and capabilities to an application. For instance a user can be a role which has read abilities while another role cold be an administrator which has access to private paths of the application and has read and write capabilities.

## Why is role based access control more scalable than discretionary or mandatory access control
* Mandatory access control depends on the system controlling access while discretionary access control depends on the user giving permissions to other for their own resources. The first is rigid and the second takes a large amount of maintenance. RBAC on the otherhand allows for various categories of access with the ability to add another role as needed. Furthermore these roles can be applied to large amounts of users in whichever way is needed
* [Source Techotopia](https://www.techotopia.com/index.php/Mandatory,_Discretionary,_Role_and_Rule_Based_Access_Control)

## Define the following terms
* Authorization
  * Authorization refers to giving a user permission to access a certain resource
  * [Source Okta](https://www.okta.com/identity-101/authentication-vs-authorization/#:~:text=Authentication%20and%20authorization%20might%20sound,permission%20to%20access%20a%20resource.)
* Role Based Access Control
  * RBAC refers to assigning users a role that permits the user access to certain resources of an application and gives them certain capabilities depending on the role
* Capabilities
  * Capabilities refer to actions the user can take based on a given role in RBAC. For instance a "user" role may have "read" capabilities while a "administrator" might have "read, write, and delete" capabilities giving them a greater spectrum of actions they can take.


[Table of Contents](README.md)