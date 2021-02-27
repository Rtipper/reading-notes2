# Class 3 Reading Notes

### 3 Real World Cases for Middleware
-
-
-

### The Route Handler is Middleware
-

### How Can Middleware End the Process and Send Data to the Browser
-

### Where Can You Inject Middleware
- Middle ware can be injected within a request upon its initial ping to the server.
- Ex: ` app.get('/person', validate, (req, res) => {
  `let name =req.query.name;`
  `res.status(200).json({ name });`
`})`
