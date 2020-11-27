Markdown Quiz

# Characters for unordered list
*
+
-

Valid format for hyperlink

[Name](URL)

Markdown Types
*word* italics
**word** Bold
* Unordered list
> Quote Block
# First level Header
& Not a markdown sign
`inline code`

Image Format
![text](Image Path)

Example
## Second level header
*very exciting* italics
[Name](URL)

# Computer Config Quiz

Good Code Editor
* Code completions
* Syntax Highlighting
* Extensions

Sequences to get list of items in folder

ls -la ~/codefellows/code102

cd ~/codefellows/code102
ls -la

cd ~
cd codefellows
cd code 102
ls -la

Version of NodeJS installed comp
10 or higher
12.19

Tree command

Display a visual layout of files and folders in the terminal

Version of NPM installed
6 or higher
6.14

# Revisions and the Cloud

Git benefits to developers
Git enables collaboration between multiple developers on a softwareproject
Git reduces risk of data loss since files are synchronized with remote repositories
git allows you to track file revisions to show a change in history

The message you write to go with a commit should contain
a brief explanation of WHY you made the changes you are committing

Once you have a set of changes you want to sync to a remote repository

1. use the git ADD command to set files to staged
2. use the git COMMIT command to take a snapshot of the staged files
3. use the git PUSH command to send your new snapsjoot of the chnages to the remote repo

What version of git is installed
2.16 or higher
2.24

What is GitHub
A collaborative web site, powered by git, with cloud-based tools for software teams
and open source software projects


# Structure Web Pages with HTML

HTML
Hypertext Markup Language

Components that comprise a standard HTML element
Attributes of the tag
content within the tags
an opening tag
a closing tag

Semantic tags are
nav
header
footer
strong
main
article

Correctly nested tags
<header>
    <nav>
        <ul>
            <li>
                <a href = "home.html">Home</a>
            </li>
        </ul>
    </nav>
</header>

ul has to come before li

HTML is used to definte the structure of a web page

# Design Web Pages with CSS
CSS 
Stands for Cascading Style Sheets

CSS rule for hyperlinks on webpage to be light blue and NOT un derlined

a {
    text-decoration: none;
    color: lightblue;
}

Complete code to make text wrap around right side of image


<!-- <html>
 <head>
   <style>
     img {
 -->       float:    **LEFT:**      
<!-- 


       width: 20px;
       padding: 5px
     }
   </style>
 </head>
 <body> 
   <img src="https://cdn.pixabay.com/photo/2017/09/09/15/46/vitamin-2732432_1280.jpg" alt="Love at sea">
   <p> 
     My bounty is as boundless as the sea, My love as deep; 
     the more I give to thee, The more I have, 
     for both are infinite. 
   </p>
 </body>
</html> -->

Match the example selector with the type of selector it represents
p { color: mauve; } Element selector
.new { color: SpringGreen; } Class selector
#sitemap { color: NavajoWhite; } ID selector
* { color: DimGrey; } Universal selector

only tag stands for element selector
.tag stands for class selector
#tag stands for ID selector
* stands for universal selector

Valid ways of setting a blue like color in CSS
#23F
hsla(211,100%,70%,.75)
rgba(37,142,255,1)
hsl(200,95%,55%)

# Dynamic web pages with Javascript
What is JavaScript
Javascript is an asynchronus dynamically type interpreted script language 
designed to make web pages dynamic and interactive

Consider the following javscript code
var a =42;
var b = '42';
which of the following is true

a == b

Which of the following is a properly formatted Javascript conditional statement
assuming all variables are already declared

if (a - b >0) {
    val = a - b;
} else {
    val = b - a;
}

In Javascript what is a variable
A variable is a way to programatically reference a previously assigned
value

Match each javascript literal value with its data type
'93' is a string
93 is a number
true is boolean
'two' is a string
4 + '2' is a string

# Programming with Javascript

Which code snippet correctly defines a function in Javascript

function helloWorld(name) {
    console.log('a new world awaits,' + name);
}

var helloWorld = function(name){
    console.log('a new world awaits, ' + name);
}

What is the advantage of using functions in javascript
Functions help us avoid repeated code
Functions make code reusable
A well-named function communicates clearly its purpose
Functions let us define the code once and then run the code whenever we 
need it

Which of the below is the bext explanation of what a functio is in javascript
A reusable set of step by step instructions potentially based on input to
potentially provide some output

Select all statements that are true about functions in Javscript
Declaring a function and invoking or calling a function need to happen seperately
Functions need to be declared before they can be invoked
Functions are invoked using parentheses

What would most likely be the correct way to invoke the function defined here in order
to display a complete sandwhich

var makeSandwich = function(bread, meat, cheese) {
  <!-- var sandwich = '';
  
  sandwich = sandwich + '<img src="' + bread + '.png">'; 
  sandwich = sandwich + '<img src="' + meat + '.png">'; 
  sandwich = sandwich + '<img src="' + cheese + '.png">'; 
  sandwich = sandwich + '<img src="' + bread + '.png">'; 
  
  return sandwich;
} -->

makeSandwich('rye', 'pastrami', 'provalone');


# Operators and Loops

Which of the following is invalid javascript code and would result in a syntax error
for ( i = 1 to 5 ) {
  console.log(i);
}

Pick the optimal type loop to utilize for each of the following use cases
Ensuring a user has entered a numeric value 
A while loop
Restricting access until a correct password is entered 
A while loop
Showing each of the products in a shopping cart 
A for loop
Displaying all the books on a digital bookshelf 
A for loop

Which code example is correctly written Javascript while loop
var answer = ''; 
while (answer !== 'S3kreT P455w0rD') {
  answer = prompt('Enter the passphrase to proceed...');
}

Which for loop will have the most iterations

for (var i = 0; i <= 8; i++) {
  console.log(i);
}

Which while loop will have the most iterations
var i = 0;
while( i <= 10 ) {
  console.log(i);
  i++;
}
