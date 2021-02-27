# Class 3 Reading Notes

### 3 Real World Cases for Middleware
- Being used for authentication and validation of user accessing a website/data.
- Being able to log a speicifc timestamp of a specific request.
- Directly interacting with a database and its contents/data.

### The Route Handler is Middleware
- By definition, they are not. If those functions are used on routing methods however, they are only handler functions.

### How Can Middleware End the Process and Send Data to the Browser
- By simply functioning, middleware will alter the request sent to the server, running in a chain through all "next" or applicable middleware. Once this is complete, it will then send data back to the browser. The middleware simply has the means to alter that initial request in some way.

### Where Can You Inject Middleware
- Middle ware can be injected within a request upon its initial ping to the server and before it reaches said server.
- Ex: ` app.get('/person', validate, (req, res) => { let name =req.query.name; res.status(200).json({ name }); })`
- Here, the `validate` is tied to the validator.js middleware

### What Can Cause the Express Error: "Request headers sent twice, cannot start a second response
- Accidently sending your request out twice to the server. Best ways to combat this, are to ensure you are retruning that request with whatever middleware you are applying before moving onto the next or finishing your request.

### VOCAB
- Middleware: a computer software that provides services to software applications beyond those available from the operating system. It can be described as "software glue".
- Request Object: retrieves the values that the client browser passed to the server during an HTTP request.
- Response Object: the object which communicates between the server and the output which is sent to the client.
- Application Middleware: middleware that is used for every request within the running of the app
- Routing Middleware: middleware that is speicifc to their identified routes within an application
- Test Driven Development: a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.
- Behavioral Testing: an Agile software development process that encourages collaboration among developers, QA and non-technical or business participants in a software project. It encourages teams to use conversation and concrete examples to formalize a shared understanding of how the application should behave.


### REFS
- https://stackoverflow.com/questions/58925276/what-is-the-difference-between-a-route-handler-and-middleware-function-in-expres#:~:text=They%20are%20not%20middleware%20functions,the%20only%20one%20callback%20function
- https://en.wikipedia.org/wiki/Middleware
- https://docs.microsoft.com/en-us/previous-versions/iis/6.0-sdk/ms524948(v=vs.90)
- https://en.wikipedia.org/wiki/Test-driven_development
- https://en.wikipedia.org/wiki/Behavior-driven_development
