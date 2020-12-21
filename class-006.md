# Reading Notes Class 6 - NODE, Express & API

### Node.js
- Node.js is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
- Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.
- The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi.
- It was designed with performance in mind and is responsible for compiling JavaScript directly to native machine code that your computer can execute.
- Node programs are executed in a browser.
- the creator of Node (Ryan Dahl) took the V8 engine and enhanced it with various features, such as a file system API, an HTTP library, and a number of operating system–related utility methods.
- This means that Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.
- Many websites will recommend that you head to the official Node download page and grab the Node binaries for your system -- use a version manager instead.
- This is a program that allows you to install multiple versions of Node and switch between them at will. 
- There are various advantages to using a version manager.
- It negates potential permission issues when using Node with npm and lets you set a Node version on a per-project basis.
- You can check that Node is installed on your system by opening a terminal and typing node -v
- If all has gone well, you should see something like v12.14.1 displayed.
- Next, create a new file hello.js and copy in the following code: console.log("Hello, World!");
- If Node.js is configured properly, “Hello, World!” will be displayed.
- As can be seen on this compatibility table, Node has excellent support for ECMAScript 2015 (ES6) and beyond. 
- Node comes bundled with a package manager called npm. 
- To check which version you have installed on your system, type npm -v.
- In addition to being the package manager for JavaScript, npm is also the world’s largest software registry.
- These build tools come in all shapes and sizes, and you won’t get far in a modern JavaScript landscape without bumping into them.
- They can be used for anything from bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking.
- And if you want to start developing apps with any modern JavaScript framework (for example, React or Angular), you’ll be expected to have a working knowledge of Node and npm.

https://www.sitepoint.com/an-introduction-to-node-js/ 
