# Code 301 | Node.JS

## Class 06 Reading Notes

### ["What is Node and When Should I Use It?", by James Hibbard](https://www.sitepoint.com/an-introduction-to-node-js/)

I. Definition: "Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime."

II. NPM = Node Package Manager: the JS package manager that node comes bundled with.

- "In addition to being the package manager for JavaScript, npm is also the world’s largest software registry."

- "There are over 1,000,000 packages of JavaScript code available to download, with billions of downloads per week."

- node_modules: "This is where npm has saved lodash [a utility library] and any libraries that lodash depends on. The node_modules folder shouldn’t be checked in to version control, and can, in fact, be re-created at any time by running npm install from within the project’s root."

III. Node's Utility

- Allows for JS to be run on a server.

- "\[I]t can be used as a scripting language to automate repetitive or error prone tasks on your PC. 

- "It can also be used to write your own command line tool, such as this Yeoman-Style generator to scaffold out new projects."

- "Node.js can also can be used to build cross-platform desktop apps and even to create your own robots."

IV. Node's Execution Model

- "Node.js, however, is single-threaded. It’s also event-driven, which means that everything that happens in Node is in reaction to an event. . . . Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior."

- "Node’s execution model causes the server very little overhead, and consequently it’s capable of handling a large number of simultaneous connections."

V. Apps for which Node Is Suited

- "Node is particularly suited to building applications that require some form of real-time interaction or collaboration," e.g., chat sites.

VI. Advantages of Node

- One language for front and back end. 

- Node speaks JSON, arguably the most important format for exchanging data on the web, so no need to reformat data.

- JS is ubiquitous, so learning to use node is readily accessible.

[<--back](301week1.md)

[<--home-->](../../README.md)
