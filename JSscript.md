# Notes on Writing a Script for a Web Page

## from _JavaScript and JQuery_ by Jon Duckett
---
I. Defining the Related Roles of HTML, CSS, and JS: "These three layers form the basis of a popular approach to building web pages called progressive enhancement."

    A. HTML: Content layer
    B. CSS: Presentation layer
    C. JS: Behavior layer

II. Creating Basic JavaScript

    A. How to use objects & methods: 
        i. document.write: don't ever actually use! `[How old is this book?]
    B. "JAVASCRIPT RUNS WHERE IT IS FOUND IN THE HTML": "When the browser comes across a <script>element, it stops to load the script and then checks to see if it needs to do anything."
    
III. Summary
    
    A. "It is best to keep JavaScript code in its own JavaScript file."
    B. "The HTML <script> element is used in HTML pages to tell the browser to load the JavaScript file (rather like the <link> element can be used to load a CSS file)."

IV. Basic JavaScript Instructions

    A. "A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon."
    B. JavaScript is case sensitive.
    C. "A statement is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon. This makes your code easier to read and follow."
    D. "The semicolon also tells the JavaScript interpreter when a step is over, indicating that it should move to the next step."
    E. "Some statements are surrounded by curly braces; these are known as code blocks. The closing curly brace is not followed by a semicolon."
    F. " You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code."
    G. Variables: 
        i. Where a script can temporarily store bits of information it needs to do its job. The interpreter can only follow explicit instructions.
        ii. Declaring a variable: keyword + name = value; e.g., var quantity = 3;
    H. Data Types
        i. Numbers: "The numeric data type handles numbers."
        ii. Strings: "he strings data type consists of letters and other characters."
        iii. Booleans: "Boolean data types can have one of two values: true or false."
    I. Rules for Naming Variables
        i. "The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number."
        ii. "The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name."
        iii. "You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something."
        iv. "All variables are case sensitive."
        v. "Use a name that describes the kind of information that the variable stores."
        vi. "If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word."
    J. Isn't var Out of date, having been replaced by let? If so, why are we still learning var?

    ![<--home-->](README.md)