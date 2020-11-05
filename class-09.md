<!-- HTML Chapter 7 Forms 144-175
Chapter 14 Lists, Tables & Forms 330-357
JS Chapter 6 Events 243 292 -->
# Class 09 Notes

## HTML Chapter 7: Forms
* HTML borrows the concept of forms to refer to a different elements that allow you to collect information from visitors to your site
* Types of form controls
* Adding text
    * Text input (single-line)
    * Password input (single-line)
    * Text area (multiple-line)
* Making Choices
    * Radio buttons
    * Check boxes
    * Drop-down boxes
* Submitting forms
    * Submit buttons
    * Image buttons
    * File upload
* Forms work by taking user input and a submit action like a button, server processes it, and sends
a new page to the browser
* A form may have several form controls and server needs to know which values correspond i.e. username = ivy

### Structure
* ```<form action = "URL" method = "get/post">``` tag carries action attribute and method
* action attributer is url for the page on the server that will receive the information in the form when it is submitted
* Forms can be sent using two methods get or post
* get adds the value from the form to the end of the url specified in the action attribute
    * Good for short form such as search boxes
    * Retrieving data from the web server no need for databases
* post method values are sent in HTTP headers and are used for 
    * File uploads
    * Long submissions
    * Contains sensitive data
    * Adds or deletes information to a database
* ```<input>``` used to create several different form controls and does not have a closing tag
    * Contains type = text, name = , maxlength =, old code may contain a size attribute
    * ```<input type = "text" name = "username" maxlength = "30">```
* input ```type = password``` will create a text box that blocks out characters
* ```<textarea>``` for multi-line text input and needs closing tag; text entered between tags will show when user loads pages
* input type radio for buttons, name, value, checked for default checked at time of load
* input type checkbox same parameters as radio button
* Drop-down list box requires select tag, name for server
    * option tag for each option, value for return value and selected for default
* Multiple select box can be created using select tag, with size attribute, you can allow multiple selections with multiple attribute
* File input box uses input tag with type file and this creates a browse button which allows user to find files
* Submit button is input tag with submit type
* Image button is input type image
* button tags allow for greater control over how buttons appear
* input type hidden shows a hidden control form
* label tag can be used before an input or can have a for attribute to associate with values
* You can group elements together using a fieldset tag helpful for longer formss
* Legend tag after a fieldset explains all the data below
* HTML5 form validation 
* Date iput requires input tag type date
* Input types also for type email and url and search
* On any text input you can place a placeholder attribute text value will show text in box

## HTML Chapter 14: Lists, Forms and Tables CSS

### Lists 
* Bullet point styles
* Unordered
    * list-style-type values: none, disc, circle, square
* Ordered
    * decimal, decimal-leading-zero
    * lower-alpha
    * upper-alpha
    * lower-roman
    * upper-roman
* Images for bullets
    * list-style-image: url("ulr")
* Positioning markers in lists
    * list-style-position: outside or inside
* List shorthand
    * list-style: position style;

### Tables 
* Table properties
    * width
    * padding
    * text-transform to convert content of table headers to uppercase
    * letter-spacing, font-size
    * border-top, border-bottom
    * text-align
    * background-color
    * :hover to highlight a table row
    * Tricks; shade every other row, bold headers, give cells padding
* Empty cells borders
    * empty-cell: show, hide, or inherit
* Gaps between cells
    * border-spacing, border-collapse: collapse or seperate

### Forms
* Styling text inputs
    * :focus pseudo class used to change background color of text input when it is being used
    * :hover
    * background-image adds a background image to the box
* Styling submit buttons
    * color, text-shadow, border-bottom, background-color, :hover
* Styling fieldsets and legens
    * width, color, background-color, border, border-radius and padding
* Aligning form controls
    * Float titles and set width
    * Set width and vertical space between each row using div
* Cursor styles
    * auto, crosshair, default, pointer, move, text, wait, help, url("cursor.gif")
* Web developer toolbar extension from chrome can show useful tools for CSS styles and apply it to an element to make life easier

## JS Chapter 6: Events
* Events are a way of indicating something has happened such as a button being clicked
* Binding stats which even you are waiting to happen and which is waiting for that event
* When an event occurs on an element it can trigger a js function making web pages feel interactive
* Event delegation can be used to monitor events that happen on all of the children of an element
* Most commonly used events are W3C DOM events although others exist


[Table of Contents](README.md)