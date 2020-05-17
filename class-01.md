# Node Ecosystem, TDD, CI/CD

## Node.js

1. Node.js is an open-source framework for writing Javascript on your operating system.
2. It is compromised of the V8 Javascript runtime and the NodeAPIs.
3. Node.js uses an event loop that is driven and non-blocking architecture - this enables Node.js to have very low overhead when it is not running.
4. Node.js runs on various platforms (Windows, Linux, Unix, Mac OS X, etc.)
5. V8 supports many features in the latest version of Javascript, called ES6 .

## package.json

1. The package.json file is used to describe and configure a Node.js package.
2. we often use npm init or npm init -y to automate the creation of this file.
3. package.json files can have a scripts field where keys can be associated with UNIX commands. This gives us the ability to create custom automation scripts

## Test-Driven Development

- It's is a process of developing and running automated test before actual development of the application .
- It's starts with designing and developing tests for every small functionality of an application.

### How to perform TDD Test
Following steps define how to perform TDD test,

- Add a test.
- Run all tests and see if any new test fails.
- Write some code.
- Run tests and Refactor code.
- Repeat.
![Image](img/tdd.png)

## Continuous Integration(CI)

1. It's is the process of regularly merging individually developed features of code into a shared repository as frequently as they are made.
2. You could simply use git to merge code into a master branch.

## Continuous Delivery(CD)

It's is the process of deploying software in short cycles by ensuring that software can be deployed at any time, CD pairs very will with advanced CI setups.

### What is the difference between a module and a package?
- A module is a single JavaScript file that has some reasonable functionality.
- A package is a directory with one or more modules inside of it and a package. json file which has metadata about the package. 

### What does the node package manager do?
Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node.js packages in your application.
It is also an online repository for open-source Node. js packages.

### Why would you want to run JavaScript code outside of a browser?
Running JavaScript inside a browser means you are interacting with Web UI (HTML and CSS components) which is displayed on a user's screen. Running JavaScript without/outside a browser means you are using node. js technology to execute your JavaScript code.

### 3 different ways to export a function from a node module

1. module.exports = {
    method: function() {},
    otherMethod: function() {},
};

2. exports.method = function() {};
exports.otherMethod = function() {};

3. let add = function (a, b) {
   console.log(a + b);
};

 module.exports.add = add;