<!-- Understanding the problem domain
JS Chapter 3: Object Literals pp. 100-105
JS Chapter 5: Document Object Model pp. 183-242 -->
# Class 06 Reading Notes

## Understanding the Problem Domain is the Hardest Part of Programming
### From "The Simple Programmer" and written by John Sonmez
* Many problem domains are like a puzzle with a blurry picture or no picture at all
* Programming is easy if you understand the problem domain
* Cut out cases and narrow focus to a particular part of the problem
* Understand a problem inside and out before you begin coding

## JavaScript Chapter 3: Object Literals (pp.100-105)
* Objects group together a set of variables and functions to create a model of something you would recognize from the real world.
* In an object variables become known as properties
* In an object functions become known as methods
* Literal notation is the easiest and most popular way to create objects
* The object is stored in a variable
* Each key is seperated from its value using a colon and each property and method with a comma
* ```var hotel = { name: 'Quay', rooms: 40, booked:25, 
    checkAvailibity: function(){ return this.rooms - this.booked;}};```
* this. function indicates that it is using the rooms and booked properties of "this" object

### Accessing an Object and Dot Notation
* You access the properties or methods of an object using dot notation, you can also access properties using square brackets.
* ```var hotelName = hotel.name;```
* ```var roomsFree = hotel.checkAvailability();```
*  or 
* ```var hotelName = hotel['name'] and var roomsFree = hotel['checkAvailability']();```

## JavaScript Chapter 5: Document Object Model

### Document Object Model (DOM)
* The DOM specifies how browsers should create a model of an html page and how javascript can access and updatethe contents of a web page in the browser window
* DOM is an object model and uses a DOM tree to illustrate html structure
    * DOM tree has each html piece as a DOM node
    * Elemnt nodes
    * Attribute nodes
    * Text nodes
* DOM is an application programming interface or API
* Accessing the DOM tree requires
    * Locating the node that represents the element
    * Use its text content, child elements, and attributes
* Step one uses code such as ```getElementsByID()```
* Step 2 involves code such as ```createElement()```
* Methods that find elements in the DOM tree are called DOM queries
* DOM queries can return one node or a collection known as a NodeList
* get element by ID and query selector (css) are single node queries
    * ```document.getElementByID('one')``` document is the object, dot operator, method
* Elements by class name, tag name and query selector all are nodeList queries
    * Live NodeList is updated when the script udates the page
    * Static NodeList is when script updates the page the NodeList is not updated. They reflect the document when the query was made
    * Two ways to select an element from a NodeList, the item() method and array sintax
    * item() method
    * ```var elements = document.getElementsByClassName('hot') if (elements.length>=1){ var firstItem = elements.item(0);}```
    * Array syntax
    * Same beginning as item() method but last section ```var firstItem = elements[0]```
* You can use a for loop to repeat actions for an entire NodeList
* When you have an element in the node you can select another element in relation to it using five properties
    * Parent node
    * previousSibling and nextSibling
    * firstChild and lastChild
* Whitespace nodes can make traversing DOM difficult because some browsers add nodes for whitespace in code

### Updating Element Content
* To work with elements you can navigate to text nodes or work with the containing element
* nodeValue property accesses text from node
* innerHTML gets/sets text and markup
* textContent gets/sets text only
* innerText gets/sets text only
* ```objectText.replace```
* textContent collects and can update content of an element it replaces the entire content and any markup.
* innerText also works but generally avoid it
* innerHTML allows for adding or removing content from HTML
* innerHTML is suited to updating entire fragments while DOM manipulation easily targets individual nodes
* DOM manipulation can be safer but requires more code and is slower
* DOM manipulation involves three steps
    * ```createElement() & createTextNode() & appendChild()```
* DOM manipulation also allows for removal of elements from the DOM tree

### Comparing Techniques for Updating HTML Content
* ```document.write()``` is simple and quick but only works when the page initially loads and is rarely used and frowned upon
* ```element.innerHTML``` uses less code, can be fast, is simple but should not be used to input content from a user
* DOM manipulation is suited to changing one element when there are many siblings, it easily allows script to add elements incrementally but it takes more code and can be slower for many items

### Cross-Site Scripting (XSS)
* Adding html to a page using innerhtml or jQuery makes user account access potentially vailable to attackers
* Even simple code can cause problems
* XSS can give attacker access to DOM, website cookies, session tokens, which all can have bad downstream results
* To defend against this you can validate input going to the server
* Escape data coming from the server and database
* Make sure users can only input characters they need to use and limit where this content will be shown on the page
* Filter or validate input and limit where user content goes
* Any content generated by uisers that contain characters that are used in code should be escaped on the server.
* All data from untrusted sources should be escaped on the server before being shown on the page
* When adding user content in JS use textContent or innerText and not innerHTML

### Attribute Nodes
* Once you have an elment node you can use other properties and methods on that element node to access and change its attributes
* ```document.getElementById('one').getAttribute('class')```
* can use getAttribute, hasAttribute, setAttribute, removeAttribute and properties can be className or ID
* You can create and remove attributes as well as changing them

### Examining DOM in Browsers
* Modern browsers come with tools that help you inspect the page loaded in the browsers and understand the structure of the DOM tree
* In chrome you can use the properties tool after inspect elements
* Firefox has similar built in tools but you can also download a DOM inspector tool that shows the text nodes. 



[Table of Contents](README.md)