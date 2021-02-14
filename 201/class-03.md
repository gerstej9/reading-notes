<!-- HTML Chapter 3 Lists pp 62-73
Chapter 13 Boxes pp 300-329

JS Chapter 4 Decisions and Loops pp 162-182 -->
# Class 03 Reading Notes

## HTML Chapter 3: Lists
* There are a lot of occasions when we need to use lists and HTML provides three types
    * Ordered lists wherre each item is numberred ```ol```
    * Unordered lists begin with a bullet point ```ul```
    * Definition lists are made up of a set of terms and their definitions
* Lists follow a specific style of code
    * Opening tag followed by li tags for each item
    * ```<ul> <li> Item </li> <ul>```
* Definition lists are slightly different
    * ```<dl>``` opening tag
    * ```dt``` for term
    * ```dd``` contains the definition
* Nested lists include creatinga list within a list and browsers will show these indented further

## HTML Chapter 13: Boxes

### General Topics
* With HTML boxes you can:
    * Control dimensions
    * Create borders
    * Set margins and padding
    * Show and hide the boxes
* Box dimensions are automatically set to hold contents
    * Width and height can be set and specified with pixels, percentage or ems
    * Pixels are usually standard, percentage is dependent on browser/window and em on text
    * Percentage can also be based on size of a box outside of a box
* Limiting width
    * min-width and max-width
    * These commands allow for changes in browser size so that boxes/text do not become too narrow or stretched out
* Limiting height
    * min-height and max-height
* Overflowing content
    * If content is larger than a box you can do two commands
    * hidden hides extra content
    * scroll adds a scrollbar for overflow content

### Box Appearance: Border, Margin, and Padding
* Boxes have three properties that can be adjusted to control appearance border, margin and padding
    * Every box has a border that seperates the edges of one box from another whether visible or not
    * Margins sit at the outside of the border between adjacent boxes
    * Padding is the space between the border of a box and the content within it, adding padding can increase readability.
* Padding and margin are important for adding space between items on a page, this is known as white space and vertical margin
* Border width controls the width of the border and can be in pixels or thin, medium, and thick
* You can also specify border-top-width or left, right, or bottom or do so in border-width by adding for arguments ```border-width:2px 2px 1px 2px;``` in clockwise order
* Border style also can be selected by all borders or one side
* Styles include ```border-style: solid, dotted, dashed, double, groove, ridge, inset, outset, hidden/none```
* Border color can also be selected by all or one side ```border-color```
* Border shorthand allows for all three to be defined in one ```border: 3px dotted cyan;```
* Padding property is usually specified in pixels, if in percentage it is percentage of window
* If width is specified for a box, padding is added onto the width of the box
* Like borders you can specify padding on each side individually
* Margin follows same rules as padding, if one box sits on top of another the larger of the two margins will be selected

### Content, Visibility, and CSS3
* Content can be centered in a box using ```left-margin``` and ```right-margin``` commands set to auto
* Internet explorer has a quirk where it includes padding and margins in the width of the box but this can be avoided by providing a DOCTYPE declaration
* ```display``` property allows you to turn inline elements into a block-level element or vice versa
    * ```inline``` causes a block level element to act like an inline element
    * ```block causes``` an inline element to act like a block-level element
    * ```inline-block``` creates an inline element flow with box qualities
    * ```none``` hides the element from the page
* Hiding boxes can be done through ```visibility``` either ```hidden``` or ```visible``` values
* CSS3 allows for border images ```border-image``` and takes three values; URL, where to slice image, and what to do with straight edges including ```stretch, repeat, or round```
* CSS3 also allows box shadows ```box-shadow``` with ```horizontal offset, vertical offset, blur distance, and spread of shadow``` as the four arguments as well as a color. Can suffice with the first two values and a color
* CSS3 allows for rounded corners using the ```border-radius``` property
* Border radius also allows for elliptical shapes if you specify different horizontal and vertical radii values

## Javascript Chapter 4: Decisions and Loops

### If...else Statements
* If...else statements checks a condition and if true executes one code block else executes another code block
* ```if(x>y){prompt();} else{alert();}```
* Statements inside an if statement must be followed by a semi-colon
* If statements can be executed with just an if statement
* A series of if statements will result in all being checked even if a match has been found

### Switch Statements
* A switch statement starts with a variable called the swich value, each case indicates a possible value for the variable and the code that should run if that variable matches true
* The statement lives in one code block and if none of the variable conditions are met then default is executed
* There is a break after each case to tell the Javascript interpreter that it has finished the switch statement
* ```switch(level){case 'one': title = 'level 1'; break; case 'two': title = 'level 2'; break; default: title ='test'; break;}```
* Switch statements have a default if none of the cases match
* If a match is found the break statement prevents any of the rest of the switch statement from running

### Type Coercion and Weak Typing
* Javascript will try to make sense of a wrong data type instead of notifying an error
* Type coercion involves converting data behind the scenes
* Javascript uses weak typing because data type for a value can change. Strong typing in other languages requires that you specify what data type each variable will be
* Type coercion can lead to unexpected values so it can be beneficial to use strict equals operators such as ```=== or !===``` instead of ```== or !=```

### Truthy and Falsy Values
* Due to type coercion values in JavScript can be treated as true or false
* False values include false, 0, empty string '', Nan(Not a number), or a variable with no value assigned
* True values include true, 1, 'carrot' strings with content, number calculations, 'true' as a string, '0' as a string, 'false' written as a string


### Checking Equality and Existence
* Because the presence of an object or an array can be considered truthy it is often used to check for the existence of an element on a page
* A unary operator returns a result with one operand such as looking for the presence of an element.

### Short Circuit Values
* Logical operators are processed left to right, they short-circuit as soon as they have a result but they return the value that stopped the processing which is not necessarily true or false
* Logical operators will not always return true or false because sometimes they will return a value treated as truthy or falsy even though its not boolean
* As soon as a truthy value is found the remaining options are not checked therefore sometimes programmers will put the code most likely to return true first in OR operations and false answers first in AND operators
* They will also place the options requiring the most processing power last just in case another value returns true and they do not need to run.

## Loops
* Loops check a condition and if true the code block will run. This repeats until condition returns false
* Three different types of loops
* For loops run for a specified number of times
* While loops are for an unspecifed amount of times so long as condition is true
* Do While loops similar to while but will always run the code at least once even if the condition is false
* Loops consist of keyword, condition counter, opening curley brace, code to execute during loop and closing curley brace
* ```for (var i = 0; i<10; i++){ document.write(i);}```
* A for loop uses a counter as a condition and is made up of three statements
    * Initialization ```var i =0;```
    * Condition ```i<10;```
    * Update ```i++```
* Two keywords are common with loops, break and continue. Break tells the interpreter to go to the next statement while continue tells the interpreter to stop the current iteration and then update and check the condition again.
* Loops are helpful for dealing with arrays because you can cycle through all the values of an array
* While loops operate similar to for loops but with a different structure
    * ```var i =1; var msg =''; while (i<10){msg += i{'x 5 =' +(i *5) + '<br/>; i++;}```
    * Two statements the first uses the +- operator meaning msg = msg +'newMsg' ```msg+=```
    * The second increments the counter variable by one ```i++```
* Do while loops are similar to a while loop but the codeblock comes first so that the code will run once no matter what and then loop while the condition is met.
* ```do{code block here; i++;} while (i>5);```


[Table of Contents](README.md)