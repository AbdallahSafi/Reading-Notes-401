# Readings: Classes, Inheritance

### Why would you want to run JavaScript code outside of a browser?

Running JavaScript without/outside a browser means you are using node.js technology to execute your JavaScript code. This type of usage of javascript typically refers to backend programming where your javascript code will interact with your database and can be used to create RESTful APIs.

### What is the difference between a module and a package?

- A module is a single JavaScript file that has some reasonable functionality.
- A package is a directory with one or more modules inside of it and a package.json file which has metadata about the package.

### What does the node package manager do?

Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node. js packages in your application. It is also an online repository for open-source Node.

### Provide code snippets showing 3 different ways to export a function from a node module

1. Export Function

```javascript
module.exports = function (msg) { 
    console.log(msg);
};
```

2. Export Function as a Class

```javascript
module.exports = function (firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = function () { 
        return this.firstName + ' ' + this.lastName;
    }
}
```

3. Export Function as variable

```javascript
function favoriteBook() {
    return { title: "The Guards", author: "Ken Bruen" };
}
module.exports.favoriteBook = favoriteBook;
```

## Document the following Vocabulary Terms:

- **ecosystem:**  The simplest definition of an ecosystem is that it is a community or group of organisms that live in and interact with each other in a specific environment.

- **Node.js:** is an open-source, cross-platform, JavaScript runtime environment that executes JavaScript code outside a web browser. 

- **V8 Engine:**  engine is an open source JavaScript that compiles JavaScript to optimized machine code before execution.

- **A module:** is a single JavaScript file that has some reasonable functionality.

- **A packag:** is a directory with one or more modules inside of it and a package.json file which has metadata about the package.

- **Node Package Manager (NPM):** is a command line tool that installs, updates or uninstalls Node. js packages in your application. It is also an online repository for open-source Node.

- **A server:** is a computer that provides data to other computers. It may serve data to systems on a local area network (LAN) or a wide area network (WAN) over the Internet. 

- **environment:** the development environment is the set of processes and programming tools used to create the program or software product. 

- **Interpreter:** is a program that executes instructions written in a high-level language. There are two ways to run programs written in a high-level language. 

- **compiler:** is a special program that processes statements written in a particular programming language and turns them into machine language or "code" that a computer's processor uses.