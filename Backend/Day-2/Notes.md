what is the difference between require() and Import keyword , while importing a package.
=> require() is the old method that used to import a package in the file and import is recently introduced. when we work on already running server's we can see that all the import statement is written in require() method.
Syntax:
const express = require("express");
const app = express();

app.get('/',(req,res)=>{
    res.send("Hello World");
})

// server listen
app.listen(3000,() => {
console.log("Server started on port 3000");
});

-listen() is used to run the server like on which URL / Port number it is running.
-req menas request given to a server.
-res means response from the server.
()=>{}, this is called an arrow function commonly used in making API's but we can also use standarded funtion() method.  
- "3000" this is used as a Port number. port number is like an address, used to communicate with the server.
 

defference between npx and npm
=> npx stands for node package Execution, which is used to execute a code or run something while npm stands for node package manager used to manage the package functionality.

// How to deploy server?

=> publish everything on the github except .env and node_modules by creating .gitignore file. it will ignore all the files written inside it. 

then login with github it on "render.com" and deploy your project there in free to test the deployment.


