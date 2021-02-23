# Class 2 Reading Notes

### Difference Between PUT & PATCH
- PUT is a method of modifying resource where the client sends data that updates the entire resource.
- It is used to set an entity’s information completely.
- PUT is similar to POST in that it can create resources, but it does so when there is a defined URI.
- PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.
- PATCH applies a partial update to the resource.
- This means that you are only required to send the data that you want to update, and it won’t affect or change anything else.
- If you want to update the first name on a database, you will only be required to send the first parameter; the first name.
- The only similarity between the two is that they can both be used to update resources in a given location.
- The main difference between PUT and PATCH requests is witnessed in the way the server processes the enclosed entity to update the resource identified by the Request-URI.

### Services/Tools for Mocking an API
- POSTMAN App
- STOPLIGHT.IO
- SWAGGER

### Swagger and APIDoc.js
- Swagger allows you to describe the structure of your APIs so that machines can read them.
- Swagger is an open-source software framework backed by a large ecosystem of tools that helps developers design, build, document, and consume RESTful Web services.
- Swagger allows you to describe the structure of your APIs so that machines can read them.
- apiDoc creates a documentation from API descriptions in your source code.
- apiDoc can be installed via the terminal.
- Unsuccessful API calls should be returned with a status 500 signifying an error along with a .catch statement.

### SOAP vs ReST
- Simple Object Access Protocol and Representative State Transfer.
- Representational State Transfer.
- Both serve as web service communication protocols.
- SOAP was long the standard approach to web service interfaces, although it’s been dominated by REST in recent years, with REST now representing more than 70% of public APIs.
- REST operates through a solitary, consistent interface to access named resources.
- Most commonly used when you’re exposing a public API over the Internet.
- SOAP, on the other hand, exposes components of application logic as services rather than data.
- REST allows a greater variety of data formats, whereas SOAP only allows XML.
- Coupled with JSON (which typically works better with data and offers faster parsing), REST is generally considered easier to work with.
- SOAP’s standard HTTP protocol makes it easier for it to operate across firewalls and proxies without modifications to the SOAP protocol itself.
- SOAP is highly extensible through other protocols and technologies. 

### VOCAB
- Web Server -- includes several parts that control how web users access hosted files. At a minimum, this is an HTTP server.
- Express -- Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
- Routing -- setting the pathways and "routes" of navigation throughout a web based application
- WRRC -- 

##### Refs
- https://swagger.io/docs/specification/2-0/what-is-swagger/
- https://apidocjs.com/
- https://stackify.com/soap-vs-rest/
