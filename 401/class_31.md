# Code 401 Class 31 Reading Notes

## Why do we not need more html pages in a multi page React app?
* We do not need more html pages in a multi page react app because we are able to use a browser router to render specific components on different paths. This has to do with how React renders to the DOM.

## If we wanted a component to show up on every page, where would we put it and why?
* If we want a component to show up on every page we put it within the browser path but outside of any specific route paths and that will result in it being rendered on every page.

## What does props.children contain?
* Props.children will contain any data that is placed between the opening and closing tags of the component within the parent.

## Define the Following Terms
* Composition
  * Composition refers to the utilization of components when building a React application
* Children/ Child Components
  * Child components refer to chunks of JSX that are used to build up a parent to render a complete application.
* Hash Routing
  * Hash routing looks for a change to window.location.hash which is the values following the url and when they change it utilizes a predetermined route to decide on what to render
* Link Routing
  * Link routing is declarative and utilizes a link or navlink tag to direct a user to another part of the page.


[Table of Contents](README.md)