<!-- HTML Chapter 3 Lists pp 62-73
Chapter 13 Boxes pp 300-329

JS Chapter 2 70-73
Chapter 4 Decisions and Loops pp 162-182 -->
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
* 
