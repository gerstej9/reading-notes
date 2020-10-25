# Class 01 Reading Notes

## HTML Chapters 1, 8, 17, & 18
### pp 2-11, 12-39, 176-199, 428-451, 452-475

## Javascript Chapter 1
### pp 11-52

## Introduction
* Javascript allows you to;
    * Acess content within webpages
    * To modify content
    * Program rules
    * React to events
    * Some examples include slideshows, forms, reloading part of a page and filtering data
* HTML and CSS Refresher
* HTML elements consist of opening tag containing attribute name and attribute value and a closing tag
    * ```<p class ="fruit">peach</p>```
* CSS rules have a selector and declaration block which consists of property name and value
    * ```.fruit{color:pink;}```

## Scripts
* A script is a series of instructions such as a recipe or manual
* To write a script you need to state your goal and list the tasks needed to complete it
    * Define the goal
    * Design the script
    * Code each step
* Code vocabulary and syntax are paramount for writing a script
* Sketching out tasks in flowcharts fcan be helpful to see how tasks fit together

## How Computers Fit in the World
* Computers create models of the world using data
* Models are made using data
* Things can be represented as objects. Each time an object is present is an "instance"
    * Objects can have:
    * Properties
    * Methods
    * Events
    * Together these create a working model of the specific object
* An event is the computer's way of sticking up its hand to say something has happened
* When a specific event happens that event can be used to trigger a specific section of code
* Scripts often use different events to trigger functionality
* Methods represent things people need to do with objects. They can retrieve or update the values of an objects properties.
    * A method is like questions and instructions that;
    * Tell you something about that object using information stored in properties
    * Change the value of one or more of that object's properties
* Web browsers are programs built using objects
* Web browsers create models of the web page they are showing and of the browser window the page is being shown in
* Window objects are the browser or tabs open and the property of the window object is the URL
* Document objects are the current web page loaded into each window
* The document object in this case represents an html page
    * Properties describe the characteristics of the current web page
    * Methods perform tasks associated with the document currently loaded in the browser
    * Events include user clicking on an element
* How a web browser sees a web page
    * Receive a page as HTML code
    * Create a model of the page and store it in memory
    * Use a rendering engine to show the page on screen
* All major browers usse a JavaScript interpreter to translate JavaScript instructions into instructions the computer can follow

## HTML, Javascript, and CSS
* HTML is the first layer and contains content
* CSS is the presentation layer
* Javascript is the behavior layer and provides interactivity
* The three layers provide the basis of progressive enhancement when it comes to building webpages
* Starting with HTML allows for focus on content
* CSS next seperates the content from design
* Javascript adds enhanced usability and the experience of interacting with the site
* Like CSS, Javascript files can be linked to in HTML
* You can also add JavaScript in the HTML between script tags

## JavaScript
* Calling a method of an object
    * Object.method(parameters);
    * ```document.write('Good Afternoon!');
    * Lots of objects like document and methods like write that will help write whole scripts
    * Javascript runs where it is found in HTML i.e. where the script element is
