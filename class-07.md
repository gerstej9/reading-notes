<!-- Domain Modeling
HTML Chapter 6 Tables pp. 126-145
JS Chapter 3: functions, Methods, and Object pp. 106-144 -->
# Class 07 Reading Notes

## Code Fellows: Domain Modeling
* Domain modeling is the process of creatinga conceptual model in code for a specific problem.
* An entity that stores data in properties and behaviors in methods is commonly
referred to as an object-oriented model
* Storing data within properties using .this ensures any newly created objects
can access that data later
* ```new``` keyword creats an object
* ```Math.random``` for generating random numbers and ```Math.floor``` to round down
* ```Math.round``` will round up or down
* ```.prototype``` allows methods to be added to a constructor functions prototype
* .prototype acts as a back up method if the function can't be found elsewheere
* .prototype allows for multiple functions to run shared code ensuring better cohesion
* When modeling a single entity that'll have many instances build self contained objects with the same attributes and behaviors
* Model its attributes with a constructor function that defines and initializes properties
* Model its behaviors with small methods that focus on doing one job well
* Create instances using the ```new``` keyword followed by a call to a constructor function
* Store the newly created object in a variable so you can access its properties and methods from outside
* Use the ```this``` variable within methods so you can access the object's properties methods from inside.

## HTML Chapter 6: Tables
* A table reperesents information in a grid format
* Basic table structure
    * ```<table>``` to create table
    * ```<tr>``` to create a row
    * ```<td>``` to create a new data entry
    * ```<th>``` for the header
    * ```<td colspan = number>``` allows for a data entry to span more than one column
    * ```<td rowspan = number>``` allows for a data entry to span more than one column
* Long tables
    * ```<thead>``` indicates header of table
    * ```<tbody>``` main entries
    * ```<tfoot>``` for the footer
* Old code
    * You sometimes will see width and cell padding specified in the table tags or thead in old code
    * The same is true for border, border color and background color

## JS Chapter 3: Functions, Methods, and Objects

### Object constructors can use a function as a template for creating objects
    * ```function Hotel(name, rooms) {this.name = name; this.rooms; = rooms}```
    * Name of a constructor function usuallyl begins with a capital letter as a reminder to use
    the ```new``` keyword when creating a new object using that function
    * Create new instances of an object using constructor function
    * ```quayHotel = new Hotel('Quay',40, 25);```
* You can add properties using ```name.new_property = ''``` notation
* ```delete name.keyword``` to delete properties
* This keyword refers to one object usally the object in which the function operates

### Arrays are Objects
* Arrays are a special type of object and hold related set of key/value pairs but each value is its index number
* The property of any object can hold an array
* ```index number 0 (accom:420, name: 'james', phone:10) access using costs[2].phone```

### Built-In Objects
* Browsers come with a set of built-in objects that represent things like the browser window and current web page shown
* Browser Object Model contains objects that represent the current browser window or tab
    * window.print();
    * window.screen.width;
    * Window object contains other objects that tell you about the browser
* Document Object Model uses objects to create a representation of the current page
    * getElementByID
    * lastModified
* Global JavaScript Objects represent things that the JS language needs to create a model of such as an object that deals only with dates and times.
    * toUpperCase()
    * Math.PI
    * All strings have index numbers to represent each character
    * Whenever you have a value that is a number you can use methods and properties of the Number object on it
        * isNan()
        * toFixed()
        * toPrecision()
        * toExponential()
* In order to work with dates you create an instance of the Date object
* Once you have created a date you can use methods to set and retrieve the time and date that it represents


[Table of Contents](README.md)