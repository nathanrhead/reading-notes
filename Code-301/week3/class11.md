# Code 301 | EJS = Enhanced JavaScript Templating

## Class 11 Reading Notes

### [An EJS Tutorial from WalkThroughCode](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

I. Introduction: the agenda for this series of six videos, including evaluating an injected variable, iterating over an array of values, and using if/else statements, layouts, and partials.

II. Getting Started

- Setup of a server

- What's new for me?

  - using a body parser.
  - setting 'views' and using __dirname to join all views.
  - setting the view engine to be EJS.

III. Evaluting Injected Variables

- response.render takes 3 parameters: the view file's name as a string, sans file path, an object of local variables, and a call-back function.

- Using opening and closing ejs tags e.g., <% %> (you can just type ejs in vs code, and it'll create the tags for you ), in your index.ejs file, you can dynamically insert values of an object using .render when responding to a client request.

- common use case: a delete call that doesn't require passing data; passing in images;

- anything can be passed in or intected.

IV. Iterating over an Array of Values

- in your ul inside ejs tags do a for(var person of people), where people is the name of the object and person is the new name of the variable, cloding the ejs tag after the closing curly.

- in the li, in between ejs tags, with the opening tag followed immediately by an equal sign, enter person.name.

- close everything before the closing ul tag with a closing curly in opening and closing ejs tags.

V. Using if/else statements: it looks the way you'd expect, only the syntax is written within ejs tags where appropriate.

VI. Layouts

- Not native to EJS, but useful.

- have to be installed as a package: npm install --save express-ejs-layouts

- the layout.ejs is the wrapper, all html with ejs tags where needed with a dash immediately after the opening tag and a body inside an additional set of ejs tags.

VII. Patials

- Native to EJS.

- Use case: nav bar, footer, something static or reusable.

- <%- include('folder/filename')> sans pathway, and badabing, badaboom.

### [The Google Books API](https://developers.google.com/books/docs/overview)

### [EJS.co](https://ejs.co/)

### [Tutorial on Using EJS to Template your Node App](https://www.digitalocean.com/community/tutorials/how-to-use-ejs-to-template-your-node-application)

[<--back](301week3.md)

[<--home-->](../../README.md)
