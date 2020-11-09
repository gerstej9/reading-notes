<!-- HTML Chapter 16 Image pp 406-427
HTML Chapter 19 Practical Information 476-492
HTML Chapter 9 ONLY pp. 201-206
MDN Article on audio and visual elements -->
# Class 11 Notes

## HTML Chapter 9 (Only pp. 201-206)
* Flash video is a popular technology used to add animations, video, and audio to websites
* Files utilized in flash are called Flash movies regardless media type
* To create a flash movie you need to purchase flash authoring from Adobe.
* Severl companies offer flash movies and players without the need to purchase the tools
* Flash movies use .fla file extension but to be used on a page needs to have a .swf extentsion
* Once exported into SWF flasah provides a code to embed in your page, previously this was done in HTML but now is more commonly done is JS
* Browsers must use a plug in to view flash known as Flash Player
* A number of factors since 2005 have meant fewer sites are written in Flash or use Flash elements
* Part of this is due to new JS libraries like JQuery, Apple does not support flash, flash does not always meet accessibility requirements and HTML5 video and audio tags allow for embedding of media.

## HTML Chapter 16 Images
* Controlling images in CSS helps to prevent making HTML markup messy
* When sizes of images repeat across a site create a class like small, medium or large and set width and height in CSS
* You can also create classes for alignment and use float in CSS
* For centering images set margin left and margin right to auto
* ```body{ background-image:url("");}``` to set a background image
* To repeat an image use background repeat with values repeat, repeat-x, repeat, y, no-repeat, fixed, or scroll
* If a background image is not repeated you can use background-position to position it on the screan which has 9 values to represent a 3x3 grid on the screen to choose position from
* Background shorthand can be used by using body: color url("") repeat position; format
* Image rollovers are the concept of having two or more images that essentially change places based on user actions utilizing image positioning
* A sprite is an image such as a logo that is used more than once for different parts of an interface
* CSS3 is going to introduce the ability to utilize gradients using the background-image command, however, right now different syntax is needed for different browsers
* To overlay text on an image you need an image that is low contrast.
* You can place a semi transparent background color behind the text to improve legibility.

## HTML Chapter 19 Practical Information
* Search Engine Optimazation is the practice of trying to help your site appear nearer the top of search engine results
* SEO involves on-page techniques like keywords in text
    * Seven key places
    * Page title, URL, headings, text, link text, image alt text, page descriptions
* Determining which keywords to use on your site can be hard
    * Brainstorm, organize, research, compare, refine, and map your keywords
* SEO also involves off-page techniques like getting other sites to link to you
* Learning about your visitor is important and can be done using Google Analytics
    * You place a code on each page of your site and a google interface will report to you user information
    * Visits, unique visits, page views, pages per visit, average time on site, date selector, and export link are some of what this provides
    * In addition which pages, landing pages, bounce rate, top exit pages, and referrers
    * There are also advanced features that can be studied more
* Domain names are your web address and you need to register them and pay an annual fee
* Web hosts are web servers that connect to the internet and host your domain
* Most hosting accounts will provide email addresses associated with the account
* Content management systems likely use a server-side programming language and database so make sure to check the hosting company supports the technologies your software needs
* Hosted services exist where you can create your own profile on their site such as wordpress and shopify, however, you will usually need to pay for a package to get an email address or other added features.

## MDN Video and Audio APIs
* Code examples are taken from MDN Webdocs
* HTML5 comes with elements for embedding media in documents
    * ```<video> and <audio>``` tags
    * ```<video controls> <source src="rabbit320.mp4" type="video/mp4"> <source src="rabbit320.webm" type="video/webm"> <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.        mp4">link to the video</a> instead.</p> </video>```
    * This is an example of code needed for a video player
* HTMLMediaElement API provides features to allow you to control video and audio player programatically
* Wrap the whole player in a div element
* Video contains two source elements so that different formats can be loaded depending on the browser being used
* Four buttons for play/pause, stop, rewind, and fastfoward
* Each button has a class name, data-icon and an aria-label to provide an understandable description
* There is also a timer div whihc will report the elapsed time when the video is playing
* For CSS use a .controls class set custom controls to hidden.Controls have an opacity of 0.5 by default.
* Lay out buttons inside the control bar using display:flex;
* Javascript is used to create interactivity with the browser and you do so by using event listeners and functions.


[Table of Contents](README.md)