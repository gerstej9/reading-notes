# Class 08 Notes

## HTML Chapter 15: Layout
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
    * ```h1{position:absolute; top 0px; left:500px; width: 250px;}``` absolute positioning
    * ```position:fixed; top:0px; left:0px; padding:10px;}```
* ```z-index:10;``` higher z-index means on top of lower index numbers, also known as stacking context

## Floats
* ```float:right;``` float places content as far right or left of box but should be used with width property otherwise it will take up entire width
* Floats can be used to place elements side by side
* clear is used to say do not touch the side of another box within the same containing element
* Containing elements that only have floats can sometimes be treated as 0 pixels tall, to overcome this you can set overflow to auto and width to 100%
* You can create multi-column websites by using width to set width of columns, margin, and float

## Sizing and Layouts
* Screen size is related to the device being used
* Screen resolution is the number of dots showing on a screen
* Page size relates to the size of the web page and width is usually 960-1000px. Try to put pertinent information in that space
* Fixed width layouts do not change size in regards to browser window and measurements are usually given in pixels.
* Liquid layouts stretch and contract as the user increases or decreases the size of their window and use percentages
* Many designers use layout grids to design pages
* 960 grid is a commonly used grid layout and offers multiple arrangements of boxes
* CSS frameworks like the 960 grid provide code for common tasks
* You can link multiple style sheets in an html or you can @import styles sheets into one master style sheet.

[Table of Contents](README.md)