# Review: ES6 Classes

### Classes are a template for creating ____.

Classes are a template for creating objects. They encapsulate data with code to work on that data

### Can a class declaration be hoisted?


Like function expressions, class expressions may be anonymous, or have a name that's different from the variable that it's assigned to. However, unlike function declarations, class declarations have the same temporal dead zone restrictions as let or const and behave as if they are not hoisted.

### How would you describe a constructor and contextual “this” to a non-technical friend?

* Constructor: It's like a blueprint that defines how an object should be created in a program.

* "this" keyword: It's a way for an object to refer to itself. It helps the object access its own properties and methods.

In simple terms, a constructor is a blueprint for creating objects, and "this" is a word that allows an object to talk about itself and use its own stuff.

## Using Express Routing

### Within Express, what does routing refer to?
Routing refers to how an application’s endpoints (URIs) respond to client requests.

### What is the difference between a route path and a route method?
A route method is derived from one of the HTTP methods, and is attached to an instance of the express class.

Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.


### When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

have more than one callback function as arguments. f next has been passed to your middleware as a parameter, it means that the previous middleware or route handler expects you to call next() to pass control to the next function. 

## Express Routing

### What is an Express Router?

 It is a mini express application without all the bells and whistles of an express application, just the routing stuff. 
### By what mean do we initialize express.Router() in an express server?
in a way similir to this:

**const** router = express.Router();

### What do we use route middleware for?

Route middleware in Express is a way to do something before a request is processed. This could be things like checking if a user is authenticated, logging data for analytics, or anything else we’d like to do before we actually spit out information to our user.