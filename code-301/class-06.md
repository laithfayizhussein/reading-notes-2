# Node JS:
## What Is Node.js?
- Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.
- This means that Node.js is a program we can use to execute JavaScript on our computers.
## How Do I Install Node.js?
- you can check that Node is installed on your system by opening a terminal and typing ` node -v.` If all has gone well, you should see something like `v12.14.1` displayed. This is the current LTS version at the time of writing.
- As can be seen on this compatibility table, Node has excellent support for ECMAScript 2015 (ES6) and beyond. As you’re only targeting one runtime (a specific version of the V8 engine), this means that you can write your JavaScript using the latest and most modern syntax
## npm:
- Node comes bundled with a package manager called npm.
- In addition to being the package manager for JavaScript, npm is also the world’s largest software registry.
- Working with the package.json File:
    - node_modules. This is where npm has saved lodash and any libraries that lodash depends on.
    -  you open the package.json file, you’ll see lodash listed under the dependencies field. By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use npm to install whatever packages it needs to run.

## What Is Node.js Used For?
- nstalling (via npm) and running (via Node) various build tools — designed to automate the process of developing a modern JavaScript application.

## The Node.js Execution Model:
- when you connect to a traditional server, such as Apache, it will spawn a new thread to handle the request. In a language such as PHP or Ruby, any subsequent I/O operations (for example, interacting with a database) block the execution of your code until the operation has completed. 
- he server has to wait for the database lookup to complete before it can move on to processing the result. If new requests come in while this is happening, the server will spawn new threads to deal with them. 

![Execution Model](./img/read-6.png)
