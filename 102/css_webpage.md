# Webpage Design Using CSS

## Understanding CSS
* CSS treat elements as if each is in their own box
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

## Using External CSS
* link elements can be used to tell browser wherer to find CSS file used to style the page, it does not need a closing tag and lives inside the head.
    * Consists of three elements
    * href specifies path of CSS file (usually in a folder called css or styles)
    * type specifies type of document linked to value should be text/css
    * rel specifies relationship between HTML page and file it is linked to, value should be stylesheet when linking to CSS files
* HTML page can use more than one style sheet by having a link element for each file

## Using Internal CSS
* CSS rules can be applied inside an HTML file by using a style element which usually sits inside the head element
* Style element should use type attribute to indicate styles specified in css and value should be text/css
* When building a webpage with multiple pages you should use an external CSS style sheet
    * Allows all pages to use same style rules
    * Keeps content seperate from design
    * Allows for changes in style across all pages

## CSS Selectors
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

## CSS Rules Cascade
* If two selectors are identical the latter of the two will take precedence over the first
* If one selector is more specific than the others, the more specific rule will take precedence over the more general
* You can add !important after any property value to indicate that it should be considered more important the other rules that apply to the same element
* Cascading rules allows for generic rules applicable to all that can be overruled for specific instances

## Inheritance
* Specifying color or font properties on the body element means they will apply to most child elements.
* Background color or border properties are not inherited by child elements
* You can force a lot of properties to inherit values from their parent elements by using inherit for the value of the properties

## Why Use External Style Sheets
* All web pages can share same style sheet
* Allows for faster loading of pages
* Easier for editing
* Makes HTML code easier to read and edit
* CSS rules can be in same page as HTML code, however, usually considered better practice to have a seperate file

## Different Versions of CSS and Browswer Quirks
* Different versions of CSS
* Some old browsers do not support every CSS property
* Some browsers display CSS properties in an unexpected way
* Test sites in different browsers to account for this
* Online tools allow for site checking with different operating systems
* Browser quirk or CSS bug refers to when a site displays different than expected

## Using Color in your Webpages
* Three common ways to specify colors plus others in CSS3
* Color terminology is important
* Contrast and making text readable
* Background color for entire webpage or parts of a page

## Foreground Color
* Color property allows you to specify the color of text inside an element
* RGB values express color in terms of red, green and blue
    * `rgb(100,100,90)`
* Hex codes are six digit codes that represent amount of red, green, and blue in a color and are preceded by a hash sign
    * `#ee3e80`
* Color names specify 147 predefined color names
    *`DarkCyan`

## Background Color
* Background color for each HTML element "box"
* Specified in the same way as foreground color
* By default most browsers have a white background

## Understanding Color
* Every color on a computer screen is generated by mixing blue, red, and green.
* You can use a color picker to determine which color to use
* RGB values are numnbers between 0-255
* Hex codes has a hash followed by six characters
* Hue is a colloquial idea of color
* Saturation refers to the amount of gray in a color
* Brightness refers to how much black is in a color

## Contrast
* Ensure there is good contrast between foreground and background so that text is legible
* Lack of contrast is particularly difficult for those with visual impairments and color blindness
* It also effects users with poor monitors of when sunlight is present
* High contrast makes reading easier, however, for large amounts of text medium contrast is better

## CSS3 Opacity, HSL and HSLA
* Opacity is introduced in CSS3 and allows for specifying the opacity of an element with a number between 0.0 and 1.0 i.e. .5 = 50% opacity
* A fourth value is required for RGBA values and that is for opacity
* Some browsers do not supoort this new RGBA format so it is important to have a fallback solid color
* HSL colors stands for hue, saturation and lightness values
    * HSL colors show hue as a color circle or slider
    * Saturation and lightness as percentage values
    * `background-color: hsl(0, 0%, 78%);`
* HSLA adds the opacity value "alpha"
    * `background-color: hsla(0, 0%, 78%, 0.5)`

[Home](README.md)

