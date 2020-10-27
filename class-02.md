# Class 02 Reading Notes


## HTML Chapter 2: Text
* When creating a web page you use tags (known as markup) that provide extra meaning and allow browsers to show structure
    * Structural markup are elements that you use to describe headings and paragraphs
    * Semantic markup provides extra information such as emphasis, quotation, meaning of acronyms and more
* HTML has six levels of headings `<h1>-<h6>`
    * h1 is used for main headings
    * h2 used for subheadings
    * h3 for sub sub etc.
    * heading size is determined by number h1 being the largest
* Paragraphs are designated by `<p>` tag
    * By default browsers will show each paragraph on a new line with space between subsequent paragraphs
* Enclosing words in `<b>` tags allows for bold 
* `<i>` tag makes characters italic
* `<sup> and <sub>` allow for super and subscript respectively
* Browsers will condense two or more spaces into one space and this is called whit space collapsing
* `<br />` is known as a line break, does not need a closing tag, and will create a new line
* `<hr />` is known as a horizontal line rule, does not need a closing tag and creates a horizontal line
* Line break and horizontal line tags are known as empty elements because they do not have closing tags and have a backslash in the only tag. It is good format to put a space between the character and backslash in the tag
* Visual editors and code viewers are different and siplay content differently but are usually part of content management systems and html editors
* Some text elements that do not affect web page structure but add extra information are known as semantic markup such as 
    * `<strong>` creates bold text
    * `<em>` puts characters in italics
    * `<blockquote>` will indent a long quote
    * `<q>` is supposeed to put quotation marks around text but does not work in internet explorer
    * `<abbr>` allows for a hovering full title to appear over the acronym
    * `<cite>` used for citation and will put text in italics, usually used for persons name
    * `<dfn>` element is used to indicate the defining instance of a new term
    * `<address>` is used to specify contact details for the author of the page, some browsers will show in italics
    * `<ins> and <del>` Show content inserted and deleted usually using underline and strikethrough
    * `<s>` element shows content no longer relevant but still showed usually with a strikethrough


## HTML Chapter 10: Introducing CSS
** CSS treat elements as if each is in their own box
* CSS allows you to create rules to control the way each box is presented
    * Such as boxes, borders, text styles, and special design elements.
* CSS associates rules with HTML elements
    * Involves selectors and declarations
    *  `p{ font-family: Arial;}` In this case p is the selector and the rest the declaration
* CSS properties affect how elements are displayed
    * CSS declarations consist of a property and value seperated by a colon
    * `color: yellow;`
    * Properties indicate aspects of element; color, font, width, height etc.
    * Values specify settings such as the type of color

### Using External CSS
* link elements can be used to tell browser wherer to find CSS file used to style the page, it does not need a closing tag and lives inside the head.
    * Consists of three elements
    * href specifies path of CSS file (usually in a folder called css or styles)
    * type specifies type of document linked to value should be text/css
    * rel specifies relationship between HTML page and file it is linked to, value should be stylesheet when linking to CSS files
* HTML page can use more than one style sheet by having a link element for each file

### Using Internal CSS
* CSS rules can be applied inside an HTML file by using a style element which usually sits inside the head element
* Style element should use type attribute to indicate styles specified in css and value should be text/css
* When building a webpage with multiple pages you should use an external CSS style sheet
    * Allows all pages to use same style rules
    * Keeps content seperate from design
    * Allows for changes in style across all pages

### CSS Selectors
* CSS selectros allow you to target rules to specific elements in an HTML document
* Universal selectors apply to all elements in the document
    * `* {}
* Type selectors match element names, targets h1, h2, h3 elements
    * `h1{}`
* Class selectors match an element whos class attribute has a value that matches the one specified after the period
    * `.note{}`
* ID slectros matches an element whose id attribute has a value that matches the one specified after the hash symbol
    * `#introduction{}`
* Child selector matches an element that is a direct child of another
    * `li>a {}`
* Descendant selector matches an element that is a descendent of another specified element
    * `p a {}`
* Adjacent sibling selector matches an element that is the next sibling of another
    * `h1+p{}`
* General sibling selector matches an element that is a sibling of another regardless of whether it is directly preceding the element
    * `h1~p {}`

### CSS Rules Cascade
* If two selectors are identical the latter of the two will take precedence over the first
* If one selector is more specific than the others, the more specific rule will take precedence over the more general
* You can add !important after any property value to indicate that it should be considered more important the other rules that apply to the same element
* Cascading rules allows for generic rules applicable to all that can be overruled for specific instances

### Inheritance
* Specifying color or font properties on the body element means they will apply to most child elements.
* Background color or border properties are not inherited by child elements
* You can force a lot of properties to inherit values from their parent elements by using inherit for the value of the properties

### Why Use External Style Sheets
* All web pages can share same style sheet
* Allows for faster loading of pages
* Easier for editing
* Makes HTML code easier to read and edit
* CSS rules can be in same page as HTML code, however, usually considered better practice to have a seperate file

### Different Versions of CSS and Browswer Quirks
* Different versions of CSS
* Some old browsers do not support every CSS property
* Some browsers display CSS properties in an unexpected way
* Test sites in different browsers to account for this
* Online tools allow for site checking with different operating systems
* Browser quirk or CSS bug refers to when a site displays different than expected

## JavaScript Chapter 2: Basic JavaScript Instructions

### JS Statements and Comments
* Scripts provide a series of instructions, each one is known as a statement and should end with a semi-colon
* Javascript is case sensitive
* Each statement starts on a new line
* Statements can be organized into code blocks using curly braces these are not followed by semi-colons
* Code blocks can be used to group together multiple statements for organization and readability
* Comments should be included in code to help yourself and others when reading it
* Multi-line comments ```/* hello*/```
* Single-line comments ```//```

### Variables
* Data can be stored as variables
* Variables can be considered short term memory because the page holds the data only while user is on the page
* Data in variables can change each time the script is run
* To declare a variable you need variable keyword and name
    * ```var quantity;```
    * Variable names should be written in camelCase if using multiple words
* Once a variable has been created you can assign a value to it, = sign is the assignement operator
    *  ```quantity = 3;```
* Until a variable is assigned it is considered undefined
* Variable shorthand is sometimes used to create variables
    * Variable is declared and values assigned in same statement
    * Three variables are declared on same line then values assigned to each
    * Two variables are declared then a third is declared and assigned on next line
    * Variable used to hold a reference to an element in the HTML page
* Variables can be changed later in the same script
* Rules for naming variables
    1. name must begin with a letter, dollar sign, underscore and not a number
    1. Name can contain letters, numbers, dollar sign, or underscored but no dashes or periods
    1. No keywords or reserved words can be used for instance var
    1. All variables are case sensitive, do not create variables with the same name but in different cases
    1. Use a name that describes the kind of information the variable stores
    1. Use camelCase when naming variables with multiple words included

### Data Types
* Numeric data
* String data includes letters and characters
* Boolean are true or false
* Variables can store numbers, strings, or booleans
* Strings are kept in quotations either single or double
* To add quotes inside either use escape character such as backslash or use the opposite quote marks to surround the string i.e. single or double

### Arrays
* Arrays are a special type of variable that store a list of variables
* Good to work with an array when you are using a list of related values
* Values in arrays are seperated by commas
*  ```var colors; colors = ['white','black','grey'];``` Called literal array technique
* Array values do not need to be the same data type in one array i.e. can be booleand, string or number
* Array constructor technique ```var colors = new Array('white','black','grey');```
* Values in array can be accessed by using index which starts at 0 ```itemOne = colors[0]``` is equivalent to first value in the array
* Length of an array ```numColors = colors.length```
* To change specific value in an array ```beige = colors[2]``` changes black to beige

### Expressions and Operators
* An expression evaluates into results in a single value
* There are roughly two types of expressions
    * Expressions that assign a valuable to a variable
    * ```var color = 'beige' ```
    * Expressions that use two or more values to return a single value
    * ```var area = 3 * 2 ```
* Expressions rely on operators which allow programmers to create a single value from one or more values
    * Assignment operators assign a value to a variable
    * Arithmetic operators peform basic math
    * String operators combine two strings
    * Comparison operators compare two values and retun true or false
    * Logical operators combine expressions and return true or false
* Arithmetic operators allow for 
    * addition +
    * Subtraction -
    * Division /
    * Multiplication *
    * Increment ++
    * Decrement --
    * Modulus % Divides two values and returns the remainder
    * Order of operations PEMDAS
* String operators only use the + symbols for adding
* Joining of two strings together is known as concatenation
* Numbers added to strings become part of the string
* Arithmetic cannot be performed on string numbers
* An arithmetic function on a string will return NaN not a number

## JavaScript Chapter 4: Decisions and Loops

### Decision Making
* Using flowcharts can help plan for when script decisions are needed to be made
* There are two components to a decision
    * An expression is evaluated which returns a value
    * A conditional statement says what to do in a given situtation
* Evaluation of a condition includes code checking current status of the script commonly done by comparing two values.
* Conditional statements are based on the concept of if/then/else

### Comparison Operators
* You can evaluate a situation by comparing two values and getting a boolean result
    * ```==``` equal to meaning a string 42 can equal a number 42
    * ```!=``` not equal to
    * ```===``` strict equal to meaning a string 42 must equal a string 42
    * ```!==``` strict not equal to same concept as strict equal
    * ```>``` greater than
    *  ```<``` less than
    * ```>=``` greater or equal
    * ```<=``` less than or equal
* ```score >= test```
* ```(score1+score2) < (test1+test2)```

### Logical Operators
* Comparison operators return true false while logical operators allow comparison of results from more than one comparison operator
    * ```(5<2) && (2>=3)```
* ```&&``` tests more than one condition, "and" operator
* ```||``` "or" operator
* ```!``` "not" operator
    * ```!(2<1)``` returns "true"
* Logical expressions are examined left to right
    * Short circuit evaluation means the operator will stop if the answer is determined after the result is no longer possible
* ```var minPass = ((score1 >= pass1) || (score2 >= pass2));```

### If Statements
* If statements check if a condition is true and if so executes subsequent code
* ```if (score > 5) {congratulate();}```
* If else statements check a condition and if true runs the first code block and if false runs the second code block
* ```if (score > 5) {congratulate();} else{encourage();}```


[Table of Contents](README.md)