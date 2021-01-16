# Class 11 Reading Notes - EJS Template

### EJS
- EJS is used to include repeatable parts of our site (partials) and pass data to our views.
- package.json will hold the Node application information and the dependencies we need (express and EJS).
- filename.ejs is how we declare the files for use as EJS.
- server.js will hold the Express server setup, configuration.
- The routes for each will also be defined in the server.js file.
- Heres how this looks in the package.json file:
{
  "name": "node-ejs",
  "main": "server.js",
  "dependencies": {
    "ejs": "^3.1.5",
    "express": "^4.17.1"
  }
}

- Express and EJS along with the dependices defined above will need to be installed via the terminal (npm install)
- Route setup in the server.js file would look like this:
// load the things we need
var express = require('express');
var app = express();

// set the view engine to ejs
app.set('view engine', 'ejs');

// use res.render to load up an ejs view file

// index page
app.get('/', function(req, res) {
    res.render('pages/index');
});

// about page
app.get('/about', function(req, res) {
    res.render('pages/about');
});

app.listen(8080);
console.log('8080 is the magic port');

- Start up the server with node server.js
- Much like HTML, EJS is broken up into specifically defined parts, known as "Partials" -- head.ejd, header.ejd and footer.ejs
- Head.ejd ex:
<meta charset="UTF-8">
<title>EJS Is Fun</title>

<!-- CSS (load bootstrap from a CDN) -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.5.2/css/bootstrap.min.css">
<style>
    body { padding-top:50px; }
</style>

- Header.ejs:
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <a class="navbar-brand" href="/">EJS Is Fun</a>
  <ul class="navbar-nav mr-auto">
    <li class="nav-item">
      <a class="nav-link" href="/">Home</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" href="/about">About</a>
    </li>
  </ul>
</nav>

- Footer.ejs: 
<p class="text-center text-muted">© Copyright 2020 The Awesome People</p>
