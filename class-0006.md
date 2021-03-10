# Class 6 Reading Notes

### What is a “Singleton”?
- a software design pattern that restricts the instantiation of a class to one "single" instance

### How the Singleton pattern can be used with Node modules, specifically with classes
- It allows for their creation without having to create multiple classes that are then used again for multiple things.

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

### VOCAB
- Router Middleware -  functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. 
- Dynamic Module Loading - Functions that are exported to the module.exports object and are then referenced only when needed
- Singleton Pattern - a software design pattern that restricts the instantiation of a class to one "single" instance
- CRUD -> REST Method Matches -
  - CREATE -> POST
  - READ -> GET
  - UPDATE -> PUT
  - DELETE -> DELETE
- Mock Testing - n approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules.


# REFS
- https://en.wikipedia.org/wiki/Singleton_pattern#:~:text=In%20software%20engineering%2C%20the%20singleton,mathematical%20concept%20of%20a%20singleton.
- https://expressjs.com/en/guide/using-middleware.html
