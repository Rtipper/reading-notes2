# Class 4 Reading Notes

### Test Driven Development
- Forces your code to be more modular because you are writing smaller and more frequent tests.
- Forces good architecture in order to make your code unit-testable.
- Documents your code better than documentation.
- Makes code easier to maintain and refactor.
- Makes collaboration easier and more efficient, team members can edit each others code with confidence because the tests will inform them if the changes are making the code behave in unexpected ways.

### beforeEach() and afterEach() in a Test Suite
- beforeEach is used as the setup to Jest testing, an allows you to test data as if it were part of a database.
- afterEach is the teardown that processes after the test is complete.
- You can use both of these to test multiple things.
- They can both handle asynchronous code in the same ways that tests can handle asynchronous code

### Test Driven Developmen Downside
- The test suite itself has to be maintained; tests may not be completely deterministic.
- The tests may be hard to write, esp. beyond the unit testing level.
- nitially, it slows down development; for rapidly iterative startup environments the implementation code may not be ready for some time due to spending time writing tests first.
- Writing good unit tests is an art form and can make or break the overall functionality if the tests are bad. 

### Primary Difference Between ES6 Classes and Constructor/Prototype Classes
- The most important difference between class- and prototype-based inheritance is that a class defines a type which can be instantiated at runtime, whereas a prototype is itself an object instance.
- A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime.
- A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child.
- A class constructor creates an instance of the class.
- A constructor in JavaScript is just a plain old function that returns an object.
- The only thing special about a JavaScript constructor is that, when invoked with the new keyword, it assigns its prototype as the prototype of the returned object.

### Why REST
- REST is a lightweight alternative to most other mechanisms, and despite being simple, REST is fully-featured, easy and straighforward to use. Nothing you can do in Web Services that can't be done with a RESTful architec. Conforming and structuring around HTTP is all the REST requires to function easily and effeciently. 

### VOCAB
- functional programming: is a programming paradigm where programs are constructed by applying and composing functions
- object-oriented programming (OOP) : a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields (often known as attributes or properties), and code, in the form of procedures (often known as methods).
- class: In object-oriented programming, a class is an extensible program-code-template for creating objects, providing initial values for state (member variables) and implementations of behavior (member functions or methods).
- super: used to call the constructor of the parent class and to access the parent's properties and methods.
- this: keyword used in some computer programming languages to refer to the object, class, or other entity of which the currently running code is a part.
- Test Driven Development (TDD): a software development process relying on software requirements being converted to test cases before software is fully developed.
- Jest: a JavaScript testing framework maintained by Facebook, Inc. with a focus on simplicity and support for large web applications.
- Continuous Integration (CI): the practice of automating the integration of code changes from multiple contributors into a single software project.
- REST: Representational state transfer (REST) is a de facto standard for a software architecture of interactive applications that use Web services.
- Data Model: an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities.

##### REFs
- https://en.wikipedia.org/wiki/Functional_programming
- https://en.wikipedia.org/wiki/Class_(computer_programming)#:~:text=In%20object%2Doriented%20programming%2C%20a,(member%20functions%20or%20methods).&text=In%20these%20languages%2C%20a%20class,classes%20is%20called%20a%20metaclass.
- https://en.wikipedia.org/wiki/Test-driven_development#:~:text=Test%2Ddriven%20development%20(TDD),software%20against%20all%20test%20cases.
- https://www.atlassian.com/continuous-delivery/continuous-integration#:~:text=Continuous%20integration%20(CI)%20is%20the,into%20a%20single%20software%20project.&text=The%20version%20control%20system%20is,style%20review%20tools%2C%20and%20more.
- https://en.wikipedia.org/wiki/Representational_state_transfer
- https://en.wikipedia.org/wiki/Data_model
- https://www.toptal.com/javascript/es6-class-chaos-keeps-js-developer-up
- https://devqa.io/pros-cons-test-driven-development/#:~:text=The%20test%20suite%20itself%20has,beyond%20the%20unit%20testing%20level.
- https://jestjs.io/docs/en/setup-teardown
