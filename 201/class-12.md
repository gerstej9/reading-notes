# Class 12 Notes

## Chart.js API
* Charts can be more visually dynamic than tables
* Chart.js is a javscript plug in that uses HTML5's canvas element to draww a graph onto the page
* Download chart.js and load into the directory you are working with then link using the script tag
* Create a canvas element in your page with canvas tag
* For line graph create a label array and a data array
* You can create bar, pie, and line graphs among many others
* Chart.js can be downloaded from GitHub

## Basic Usage of Canvas
* Canvas tags have two attributes width and height but can be changed in CSS
* Provide fallback content for canvas for older browsers that don't support it. You can do this with text or a static image
* Canvas allows for 2D or 3D rendering
* getContext() function is used to obtain rendering context and its drawing functions such as 2d.
* You can also use an if else statement for examining whether browsers support canvas and supplying fallback content if not
* Use draw() function to draw out the canvas
* You can also set draw function to commence on a certain action like onload or window set interval

## Drawing Shapes with Canvas
* Canvas operate on a grid coordinate space
* To draw rectangles fillRect(x,y,width,height) or strokeRect or clearRect. Position relative to top left of rectangle
* Paths are a list of points connected by straight or curved lines with potentially different widths and colors.
* beginPath() tp start and future commands operate within. closePath adds a straight line to the path
* stroke draws the shape by adding its ouline
* fill fills the contents
* moveTo function moves to x,y coordinates
* lineTo method for straight lines
* arc() x, y, radius, startAngle, endangle, antiClockwise or arcTo() methods require x1,y1,x2,y2, and radius)
* Bezier curves can be cubic or quadratic, quadratic uses one point of control and bezier cur to uses two points of control
* Create functions when you can for repeating shapes
* Path2D API can be used as well

## Applying Styles and Color
* fillStyle = color for fill
* strokeStyle = color for outlines
* These become the style for all future shapes until changed
* You can create color palletes by changing rgb values in a for loop
* globalAlpha = transparencyValue, you can add fourth value in rgba to add transparency index
* Line commands
    * lineWidth
    * lineCap
    * lineJoin
    * miterLimit
    * getLineDash
    * setLineDash
    * lineDashOffset
* Can create gradients in strokeStyle or fillStyle with canvasGradient
* createLinearGradient
* createRadialGradient
* createPattern(image, type) can repeat x, y, all, or none
* Shadows using shadowOffset, shadowBlur and shadowColor
* You can fill canvas based on isPointInPath or other fill rules using nonzero and evenodd rules

## Drawing Text
* fillText( text, x, y [, maxWidth])
* strokeText (text, x, y, [, maxWidth])
* font = value
*  text-align
* textBaseline for positioning
* direction
* measureText allows you to get TextMetrics


[Table of Contents](README.md)