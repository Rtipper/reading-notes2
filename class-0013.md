# Class 13 Reading Notes -- Update/Delete

### Sending Form Data
- Once a form of data has been validated on the client-side, it is okay to submit the form.
- Where does the data go, and how do we handle it when it gets there?
- A client (usually a web browser) sends a request to a server, using the HTTP protocol. 
- The server answers the request using the same protoco.
- An HTML form on a web page is nothing more than a convenient user-friendly way to configure an HTTP request to send data to a server. 
- This enables the user to provide information to be delivered in the HTTP request.
- The `<form>` element defines how the data will be sent.
- All of its attributes are designed to let you configure the request to be sent when a user hits a submit button.
- The two most important attributes are `action` and `method`.
- The `action` attribute defines where the data gets sent.
- Its value must be a valid relative or absolute URL.
- If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.
- It's possible to specify a URL that uses the HTTPS (secure HTTP) protocol.
- When you do this, the data is encrypted along with the rest of the request, even if the form itself is hosted on an insecure page accessed using HTTP.
- On the other hand, if the form is hosted on a secure page but you specify an insecure HTTP URL with the action attribute, all browsers display a security warning to the user each time they try to send data because the data will not be encrypted.
- The method attribute defines how data is sent.
- The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the `GET` method and the `POST` method
- Each time you want to reach a resource on the Web, the browser sends a request to a URL.
- An HTTP request consists of two parts: a header that contains a set of global metadata about the browser's capabilities, and a body that can contain information necessary for the server to process the specific request.
- The `GET` method is the method used by the browser to ask the server to send back a given resource.
- Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.
- The `POST` method is a little different. 
- It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.
- HTTP requests are never displayed to the user but can be viewed in with the inspect tool.
- PHP offers some global objects to access the data. 
- Assuming you've used the `POST` method, the following example just takes the data and displays it to the user.
