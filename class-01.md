# Class 01 Reading Notes

## HTML & CSS Chapter 1
* Describes the structure of web pages
* HTML pages are text documents
* Tags act like containers and are often referred to as elements
* Opening tags and closing tags
* Attributes provide more information about elements such as names and values
* Web page source code is viewable through web browsers
* To learn HTML you need to know what tags are, which you can use, where they can go and what they can do

## HTML & CSS Chapter 8
* HTML has evolved through several versions since its creation
* DOCTYPE declares which version of HTML a web site is using
* Utilize comments when coding websites
* ID attributes allow elements to be uniquely stylized and are also known as global attributes
* Class attributes can be used to identify several elements
* Block elements start on a new line ( h1, p, ul, li)
* Inline elements appear on the same line as neighboring elements such as (a, b, em, img)
* Grouping text and elements in a box can be achieved through div and allows for sectioning of a page
* Span element acts as an inline version of div and is used to differentiate inline conten
* Class or an id are usually used with span
* iframe allows for a window inside a page or in other words an inline frame, needs a src for url and height and width
* iframes can have scrolling (yes, no, or auto), frameborders ( 0 or 1), or in HTML5 be seamless
* meta element lives inside the head and does not have closing tag, not visible to users but contains information about web page. 
* meta elements use name attribute to provide description, keywords, and robots which are often used by search engines. 
* meta elements use http-equiv to define author, pragma, and expiration
* Escape characters can be used to show characters otherwise used in HTML, such as ampersand escape character is `&gt;`

## Chapter 17
* HTML 5 adds new elements for dividing page
* Header and footer
* Navigation (nav)
* Article element acts as a container for sections of a page that can stand alone
* Aside element has two purposes, when used inside an article it has information related but not essential to the artical. When used outside an article it is a container for content related to the entire page such as links to other sections of the site
* Section element refers to groups of similarly related content and typically when each section has its own heading
* hgroup element is to group together one or more h1 through h6 elements so they are treated as one heading
* figure refers to images, videos, graphs, diagrams, code samples etc. that are refered to in the main flow, usually should have a figcaption as well to provide text description.
* div is revised to group together related elements when no other suitable grouping element is available. 
* HTML5 uses a elements around a block level element to contain child elements allowing you to turn an entire block into a link
* Older browsers need help with HTML5 sites meaning you need CSS code to account for this. Work arounds also include HTML.shiv or HTML.shim

## Chapter 18
* Websites should be designed for target audience
    * Age range
    * Gender
    * Location
    * Web familiarity
    * Individuals vs. companies
    * It can be helpful to create fictional visitors to your website
* Consider why visitors will come to your wbsite
    * Key motivators
    * Specific goals
* What are visitors trying to achieve on your website i.e. purchasing an item
* Provide the needed information to visitors
    * Brand identity
    * Products or services rendered
    * Features offered
    * What makes you special
    * FAQ
* Determine how often visitors will come to your site
    * Need to know how often to update your website
    * Return purchases and inventory levels
    * Subject matter updates

* Site Maps
    * Organization of information into sections or pages
    * Card sorting is a potentially helpful technicque for building a site map
    * Usually contains a homepage and potentially section homepages
    * Organize information in a way that public will understand
    * Repeat important information on multiple pages as needed

* Wireframes
    * A simple sketch of information that needs to be included on each page
    * Do not include color scheme, font choices, backgrounds or images
    * Focus on information
    * Present wireframes to clients before designs to ensure all information is presented correctly

* Design
    * Organize and prioritize content
    * Make certain features distinct from surrounding content
    * Create a visual hierarchy to attract attention
    * Group content into blocks or chunks to make visual simpler
    * Stylize information so that groups styles represent certain types of information

* Visual hierarchy
    * Gets across key message to a user skimming the page
    * Size (large vs. small)
    * Color (bright vs. dark)
    * Style (different vs. similar)
    * Utilizes visual contrast

* Grouping and similarity
    * Proximity
    * Closure
    * Continuance
    * White space
    * Color
    * Borders
    * Consistency
    * Headings

* Designing Navigation
    * Concise
    * Clear
    * Selective
    * Context
    * Interactive
    * Consistent


## Javascript $ JQuery Chapter 1
### Introduction
* Javascript allows you to;
    * Acess content within webpages
    * To modify content
    * Program rules
    * React to events
    * Some examples include slideshows, forms, reloading part of a page and filtering data
* HTML and CSS Refresher
* HTML elements consist of opening tag containing attribute name and attribute value and a closing tag
    * ```<p class ="fruit">peach</p>```
* CSS rules have a selector and declaration block which consists of property name and value
    * ```.fruit{color:pink;}```

### Scripts
* A script is a series of instructions such as a recipe or manual
* To write a script you need to state your goal and list the tasks needed to complete it
    * Define the goal
    * Design the script
    * Code each step
* Code vocabulary and syntax are paramount for writing a script
* Sketching out tasks in flowcharts fcan be helpful to see how tasks fit together

### How Computers Fit in the World
* Computers create models of the world using data
* Models are made using data
* Things can be represented as objects. Each time an object is present is an "instance"
    * Objects can have:
    * Properties
    * Methods
    * Events
    * Together these create a working model of the specific object
* An event is the computer's way of sticking up its hand to say something has happened
* When a specific event happens that event can be used to trigger a specific section of code
* Scripts often use different events to trigger functionality
* Methods represent things people need to do with objects. They can retrieve or update the values of an objects properties.
    * A method is like questions and instructions that;
    * Tell you something about that object using information stored in properties
    * Change the value of one or more of that object's properties
* Web browsers are programs built using objects
* Web browsers create models of the web page they are showing and of the browser window the page is being shown in
* Window objects are the browser or tabs open and the property of the window object is the URL
* Document objects are the current web page loaded into each window
* The document object in this case represents an html page
    * Properties describe the characteristics of the current web page
    * Methods perform tasks associated with the document currently loaded in the browser
    * Events include user clicking on an element
* How a web browser sees a web page
    * Receive a page as HTML code
    * Create a model of the page and store it in memory
    * Use a rendering engine to show the page on screen
* All major browers usse a JavaScript interpreter to translate JavaScript instructions into instructions the computer can follow

### HTML, Javascript, and CSS
* HTML is the first layer and contains content
* CSS is the presentation layer
* Javascript is the behavior layer and provides interactivity
* The three layers provide the basis of progressive enhancement when it comes to building webpages
* Starting with HTML allows for focus on content
* CSS next seperates the content from design
* Javascript adds enhanced usability and the experience of interacting with the site
* Like CSS, Javascript files can be linked to in HTML
* You can also add JavaScript in the HTML between script tags

### JavaScript
* Calling a method of an object
    * Object.method(parameters);
    * ```document.write('Good Afternoon!');```
    * Lots of objects like document and methods like write that will help write whole scripts
    * Javascript runs where it is found in HTML i.e. where the script element is

[Table of Contents](README.md)