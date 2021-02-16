# Code 401 Class 02 Reading Notes

## Node.js and Express
* Node.js is a runtime environment for javascript that is single-threaded and runs on Chrome's V8
* Express is a node web framework that allows node to perform REST actions or in other words HTTP related actions such as get, post, put, delete
* Express requires three snippets of code in node, require, .use/.get, and .listen
* The first imports express, the second provides the route path and the third starts the server on a specified port
* Express is capable of using various forms of middleware, packages availabe through npm that allow for further functionality.
* In addition users can create their own functionality and import it into files using module.exports function
* Express allows for asynchronous APIs, route handling and built in error handling.
* In addition express works with templating agents such as mustache or ejs to create page content.
* Express can also interact with databases such as PostgreSQL and MongoDB.
* Express is considered an unopinionated framework because there are many ways to achieve a certain goal and therefore it has great flexibility.
[Source MDN Webdocs](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

## npm
* npm stands for node package manager and is a large repository of packages that offer functionality in node.
* Developers can create packages and upload them to npm and others can access them through the npm command line interface
* Some packages have very niche functionality while others are widely used
[Source npm docs](https://docs.npmjs.com/about-npm)

## TDD
* TDD stands for test-driven development and is a structure used by tech companies to ensure bug free code.
* While TDD may take slightly longer the time spent testing often is rewarded by the lack of time needed for fixing bugs in the long run
* TDD has become common place in many developers lives and is part of AGILE.
* TDD is a skill that is acquired through practice and while beginning coders can create a small test and create code to pass it, more advanced coders are able to plan out test suites for each step of whole projects
* Individual and group mistakes can be made with TDD and it is important to make sure that everyone as an individual and groups as a whole know how to properly implement TDD for it to be most effective.
[Source Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))

## CI/CD
* CI stands for continuous integration and it is the process of code passing testing when it is uploaded to a central repository so that merge conflicts are less likely to arise and code is synchronized more often. This prevents branch merging from becoming unwieldly.
* CD is continuous development which is a result of continuous intergration. Because code is constantly being tested in chunks before being intergrated, code can then be deployed bug free relatively easily at shorter intervals. 
* CD also stands for continuous deployment which is a result of continuous intergration and continuous development.
[Source Github Professional Guides](https://www.youtube.com/watch?v=xSv_m3KhUO8)


[Table of Contents](README.md)