# angular

Hands-on tutorials based on official documentation of Angular.

<code>node --version</code>

<code>sudo npm install -g @angular/cli</code>

<code>ng version</code>

If you receive a ready made project

<code>npm install</code>

<code>ng serve</code>

# components

basic building blocks

<code>ng generate component housingLocation --standalone --inline-template --skip-tests </code>

# interfaces

- custom data types for your app
- you can define properties that represent data about some component for example

<code>ng generate interface housingLocation</code>

# @Input()

- inputs allow components to share data
- direction of data sharing is from parent component to child component
- for more details check <a href="https://angular.io/guide/inputs-outputs">HERE</a>

# ! non-null assertion operator

- value of this property won't be null or undefined

# Property binding

- adding property binding to a template and use it to pass dynamic data to components
- for more details check <a href="https://angular.io/guide/property-binding">HERE</a>

# Interpolation

- in order to display dynamic data in a template
- for more details check <a href="https://angular.io/guide/interpolation">HERE</a>

# \*ngFor

- use this directive in templates in order to display dynamically repeated data in a template
- for more details check <a href="https://angular.io/guide/built-in-directives#ngFor">HERE</a>

# Angular services

Angular services provide a way for you to separate Angular app data and functions that can be used by multiple components in your app. To be used by multiple components, a service must be made injectable. Services that are injectable and used by a component become dependencies of that component. The component depends on those services and can't function without them.

# Dependency injection

Dependency injection is the mechanism that manages the dependencies of an app's components and the services that other components can use.

<code>ng generate service housing --skip-tests</code>

# Routing

Routing is the ability to navigate from one component in the application to another. In <a href="https://angular.io/guide/router-tutorial#using-angular-routes-in-a-single-page-application">Single Page Applications (SPA)</a>, only parts of the page are updated to represent the requested view for the user.

The <a href="https://angular.io/guide/router-tutorial">Angular Router</a> enables users to declare routes and specify which component should be displayed on the screen if that route is requested by the application.

# Routing with route parameters

- Route parameters enable you to include dynamic information as a part of your route URL.
- For example you can use an id as parameter, as in this tutorial.
- use route parameters to pass data to a route
- use routerLink directive to use dynamic data to create a route
- use route parameter to retrieve data from a service to display specific information to UI

# ? optional chaining operator

if value is null or undefined the app does not crash

# Forms

- to collect user data
- after data collecting they are sent to a service of the app
- then service writes data to somewhere else, in this example it writes them to the browser's console log

# ?? nullish coalescing operator

- to assign default values if values in null

# Event binding

- Angular uses parentheses syntax around the event name to define events in the template code.
- You can bind to browser events and custom events

# Search functionality

- search through the data provided and display only the results that match the entered term

# template reference variable

- use a <a href="https://angular.io/guide/template-reference-variables">template reference variable</a> to get access to the HTML element as its value

# HTTP communication

- use a JSON server that your app will communicate with over HTTP
- the HTTP request will simulate the experience of working with data from a server

<code>npm install -g json-server</code>

flag -g helps you by running the latter command from every directory you are in

<code>json-server --watch db.json</code>

- in your web browser, navigate to http://localhost:3000/locations

# fetch()

- for more advanced use cases consider using HttpClient provided by Angular
