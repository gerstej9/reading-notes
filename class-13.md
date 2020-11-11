# Class 13 Notes
Reading from Dive Into HTML

## Past, Present, and Future of Local Storage for Web Applications
* Persistent local storage historically has given native client applications an advantage over web applications
* Cookies were invented early in web's history and can be used for persistent local storage of small amounts of data but have three downsides
    * Cookies are included with every HTTP request thereby slowing down web application
    * They send data unencrypted over the internet unless entire web app is served over SSL
    * Cookies are limited to 4kb of data
* Before HTML 5 attempts to solve the local storage issues were unsuccesful

### History
* Internet explorer was the first "great" browser and used userData in DHTML Behaviors
* This allowed web pages to store up to 64kb of data per domain.
* Adobe Flash 6 created a feature known as "Flash cookies" that allowed for 100kb of storage. This evolved and eventually become a part of Dojo Toolkit as dojox.storage
* Google created Gears which allowed API to an embedded SQL database that could store unlimited amounts of data per domain in SQL database tables
* dojox.storage evolved even more over a couple years to provide a unified interface to different plugins and APIs so that it could auto-detect Adobe Flash, Google Gears, Adobe AIR and an early prototype of HTML5 storage
* All these solutions were dependent on either a single browser or third-party plugins

### HTML5 Storage
* HTML5 storage is a specification known as Web Storage, certain browser vendors also refer to it as Local Storage or DOM Storage
* Local Storage is a way for web browsers to store named key/value pairs. This data persists even after you .leave the website, close the tab, exit your browser etc.
* Unlike cookies this data is never transmitted to a remote web server
* Unlike previous solutions this one is implemented natively in web browsers
* You can acess this storage with ```localstorage``` object in HTML5 on the global window object. You should check whether a browser supports it
* You can use "Modernizer" to check for browser support

### Using HTML5 "Local" Storage
* You store data as key/value pairs, the key is a string and the data can be any type supporte4d by JS such as strings, booleans, intergers or floats.
* Data is sstored as a string os if storing or retrieving anything other than strings you need to use functions such as parseInt or parseFloat for retrieved data
* Calling ```setitem()``` will overwrite a key if it already exists
* Calling ```getItem()``` with a non-existent key will return "null"
* You can use localstorage as an associative array
* ```void clear()``` allows deletion of all local storage or ```removeItem()``` to remove a singular item
* You can get total number of values in storage area and iterate through all of them by index

### Tracking Changes to Local Storage
* To track when storage area changes you can add an event listener to the event "storage"
* In internext explorer the callback function is not called with a storagEvent object but a widonw.event
* The variable e will be a storageEvent object with the properties;
    * .key a string that was the named key for the pair
    * .oldValue any data type the previous value or null
    * .newValue any data type the current value or null if removed
    * .url or .uri string type the page which called a method that triggered this change
* The storage event is not cancelable, there is no way to stop the change from occurring

### Limitations in Current Browsers
* 5 megabytes is how much each origin gets by default
* "QUOTA_EXCEEDED_ERR" is an exception that will show up if you exceed your storage quota of 5mb
* You cannot get more storage space

### Local Storage in Action
* In a game example, every time a change in the game occurs the game state is saved to local storage
* On page load instead of a new game being called it calls resume game function and uses local storage to populate previous game state
* Data is stored as strings so when retrieving it is extra important to make sure you convert it

### Beyond Key-Value Pairs
* There are competing visions for the future of HTML5 storage
* SQL, or more properly web SQL Database, is one version that allows backend database programming using JS, it is currently implmented by four browsers and platforms
* SQL has issues with standardization
* Another competing vision is the Indexed Database API known as IndexedDB
* Similar to SQL but main difference is store has no structured query language
* As of now it has only been implemented in a beta version of Firefox 4


[Table of Contents](README.md)