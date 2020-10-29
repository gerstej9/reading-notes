# Class 04 Reading Notes

## HTML Chapter 4: Links
* Links allow for "surfing" or "browsing" of the web
    * Link between internal pages
    * Other webpages
    * Different parts of the same page
    * Open a new browser
    * Start a program
* Writing a link ```<a href="https://">Title</a>```
* To link to external sites you use an absolute URL
* To link internally you use a relative URL
* Directory structure is important for websites with multiple pages
* The top level is the root folder and contains the index, files related to other pages are held in subsequent folders
* Sub-folders will also contain an index.html relative to that sub-page
* Relative URLs tell your browser where to find certain files
* Email links ```<a href= "mailto:email@email.com">Email</a>```
* Target opens links in a new window ```<a href="https://" target ="_blank">Link</a>```
* Linking to a specific part of the same page ```<a href="#id">Title</a>```
* To link to a specific part of another page ```<a href="https:/#id">URL</a>```

## HTML Chapter 15: Layout (Focus on pages 358-364)
* CSS treats each HTML element as if it is in its own box, this will either be block-level box or an inline box
    * Block level starts on new line h1, p, ul, and li tags are examples
    * Inline flows in between surrounding text img, b, and i tags are examples
* If one block level element sits inside another block level element then the outer box is known as the containing or parent element
* CSS has positioning schemes that allow for control of layout of a page; normal flow, relative positioning and absolute positioning. You can specify the positioning scheme and also ```float``` elements with the float property
* Normal flow shows every block level element on a new line moving downward and this is default
* Relative positioning moves an element from a position in normal flow shifting it to the top, right, bottom or left of where it would have been place without affecting surrounding elements
* Absolute positioning positions the element in relation to its containing element. Absolutely positioned elements move as a user scrolls up and down the page
* fixed positioning is a form of absolute positioning that positions the element in relation to the browser window as opposed to a containing element, these do not affect position of surrounding elements and do not move during user scroll
* Floating elements allow you to take that element out of normal flow and position it to the far left or right of a containing box, it will become a block level element aroun d which other content can flow
* ```box offset``` property tells the browser how far from the top, bottom, left, or right it should be placed
* When you move any element from normal flow, boxes can overlap. The ```z-index``` property allows you to control which appears on top
* ```position```
    * ```position:static``` normal flow
    * ```p.example{position:relative; top: 100px; left:100px;}``` relative positioning
    * ```h1{position:absolute; top 0px; left:500px; width: 250px;}`` absolute positioning
    * ```position:fixed; top:0px; left:0px; padding:10px;}```
* ```z-index:10;``` higher z-index means on top of lower index numbers, also known as stacking context
* ```float:right;``` float places content as far right or left of box but should be used with width property otherwise it will take up entire width
* Floats can be used to place elements side by side

## JavaScript Chapter 3: Functions, Methods, and Objects
* Functions and methods consist of a series of statements that have been grouped together because they perform a specific task. Methods are created inside and are part of a specific object
* Objects are used to create models, built in objects are a set that come with a browser
* You declare, and call a function and it contains parameters needed as input and returns a value
* ```function sayHello(){document.write('hello');}``` declares a function
* ```sayHello();``` calls the function
* Some functions take paramenters ```getarea(width, height)```
* When you input the parameters they are known as arguments
* ```return x``` how to return a value or variable
* You can return multiple values including an array
* Function declaration and function expression are similar ways to create functions but are processed by the interpreter differently ```function area``` vs. ```var area = function```
* Immediately invoked function expressions IIFE or "iffy" results in an calling and declaring a function simultaneously ```var area = (function(){}())``` requires a final parentheses and grouping operator
* Variable scope refers to where a variable is declared and therefore where it can be used
* Local variables are declared in a function and are function level variables
* Global variables are declared outside of a function and can be used globally
* Global variables use more memory and can cause naming collisions in pages where multiple people are contributing code

## Pair Programming
* Pair programming is the concept of two coders sharing one workstation
* Consists of the driver who is typing and the navigator who uses words to guide
* Pair programming touches on explaining what code does, listening to guidance, reading others code and writing code
* Pair programming has the following six benefits
    1. Greater efficiency
    1. Engaged collaboration
    1. Learning from fellow students
    1. Social skills
    1. Job interview readiness
    1. Work environment readiness


[Table of Contents](README.md)