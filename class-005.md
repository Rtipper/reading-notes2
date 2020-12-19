# Class 05 Reading Notes - Heroku Deployment

### Heroku / Node.js
- When installation completes, you can use the heroku command from your terminal.
- On Windows, start the Command Prompt (cmd.exe) or Powershell to access the command shell.
- Use the heroku login command to log in to the Heroku CLI:
- $ heroku login
heroku: Press any key to open up the browser to login or q to exit
 ›   Warning: If browser does not open, visit
 ›   https://cli-auth.heroku.com/auth/browser/***
heroku: Waiting for login...
Logging in... done
Logged in as me@example.com
- This command opens your web browser to the Heroku login page.
- If your browser is already logged in to Heroku, simply click the Log in button displayed on the page.
- This authentication is required for both the heroku and git commands to work correctly.
- Check that you have the prerequisites installed properly.
- Type each command below and make sure it displays the version you have installed.
- If no version is returned, go back to the introduction of this tutorial and install the prerequisites.
- All of the following local setup will be required to complete the “Declare app dependencies” and subsequent steps.
- This tutorial will work for any version of Node greater than 8 - check that it’s there:
$ node --version
v12.16.3
- npm is installed with Node, so check that it’s there.
- If you don’t have it, install a more recent version of Node:
$ npm --version
6.14.4
- Install Git

### Node.js for Beginners
- Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications.
- It's written in JavaScript and can be run within the Node.js runtime on any platform.
- It needs to be installed
- Creating a server is done through the terminal in JS.
- Always make sure you run back and check to see that it's working by going to the web browser and testing.
- Suppose your laptop's IP address within your local network is 192.168.1.101.  You can connect to your server through the 3000th port (for this particular example) by typing http://192.168.1.101:3000/ in your browser.
- WWW is for "World Wide Web" and we will turn your local server into a world wide server.
- Heroku is a cloud platform as a service 
- It allows you to deploy your web server, so everyone could see how awesome you are as a web developer.
- You need to create an account on developer's site and install Heroku.
- There is also instruction on Heroku's site that can explain you how to run your first simple web server, which returns you the "Hello, World!" string.
- Nearly all of this can be built within 50 base lines of code.
