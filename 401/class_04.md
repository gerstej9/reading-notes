# Code 401 Class 04 Reading Notes

## Name 3 Advantages of Test Driven Development
* Reductions in defect rates
* Reduction in effort in final project phases
* Anecdotal reports of improved design quality in code and higher technical quality
* [Source Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))

## In what case would you need to use beforeEach() and afterEach() in a test suite
* beforeEach() and afterEach() are beneficial to use when you are running many tests that need the same task done before testing and the same task done after testing.
* For instance if something needs to be initialized before or cleared after each test you can utilize these functions once to keep your code dry.
* [Source Jest.io](https://jestjs.io/docs/en/setup-teardown)

## What is one downside of Test Driven Development
* Test driven development is dependent on the quality of tests written by the developers themselves. It is possible that coders do not write strong enough tests, do not have enough coverage, do not test frequently enough or write overly trivial tests.

## What is the primary difference between ES6 classes and Constructor/Prototype Classes
* "Class inheritance defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance".
* [Source Justen Roberston](https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up#prototypical-inheritance)

## Why REST?
* REST is popular because it uses standard HTTP requests
* REST also allows flexible data outputs such as JSON formatted data
* REST is beneficial for stateless applications
* REST uses little bandwidth comparatively
* [Source Guru99](https://www.guru99.com/comparison-between-web-services.html)

## Define the following terms
* Functional Programming
  * Functional programming(FP) is "the process of building software by composing pure functions... FP is declarative rather than imperative...which is in contrast with object oriented programming (OOP)".
  * [Source Eric Elliot Medium ](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
* Object Oriented Programing (OOP)
  * Object oriented programming is the concept of using objects to model "real world things that we want to represent inside our programs."
  * [Source MDN Webdocs](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object-oriented_JS)
* Classes
  * Classes are a template for creating objects and are built in prototypes. ES6 has it's own form of classes as well
  * [Source MDN Webdocs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
* ```super```
  * "The super keyword is used to access and call functions on an object's parent"
  * [Source MDN Webdocs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super)
* ```this```
  * The this keyword stands for a value which is determined based on how a function is called. "this" can be in reference to global, function, or eval contexts and in strict mode can be any value
  * [Source MDN Webdocs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this)
* Test Driven Development
  * Test driven development is the concept of testing code as it is written to make intergration easier and to allow smooth development while code is being created. It depends on the use of testing code throughout the development as opposed to focusing primarily on testing in the final phases of development
  * [Source Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))
* REST
  * REST is an architectural style that is a RESTful service and allows for the use of HTTP verbs GET, POST, PUT,. and DELETE. It stands for Representational State Transfer.
  * [Source Guru99](https://www.guru99.com/comparison-between-web-services.html)
* Data Model
  * Data models, I believe, are the layouts present in constructor functions and classes that determine how and what data will be contained in an object
  * [Source Dev.to](https://dev.to/junior/class-based-data-model-in-javascript-4fc9)
  

[Table of Contents](README.md)