# Day 6 Readings : Problem Domain, Objects, and the DOM

## [Understanding The Problem Domain Is The Hardest Part Of Programming](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

I. "What is the hardest thing about writing code?": the problem domain

II. Short of defining the problem domain--which is what should have happened first thing in this limpid article--here are the difficulties that characterize the problem domain or are created by it:

    A. "The real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint."
    B. "As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it." At CF, they like to call this "ambiguitiy," though this term is, at best ambiguously applied here.

III. "Programming is easy if you understand the problem domain." [At this early point in my expensive studies, this statement seems, at BEST, disingenuous. Good thing no one but me is going to read these notes. I'm talking to you, future self.]

    A. This is a stupid article. He poo-poos the waterfall approach, where he was given all the specs and possible uses in advance and found that, in this context, code was easy to write;
    B. But, then, says, "Programming is easy if you understand the problem domain. . . . I’ve spent days trying to implement a feature only to finally go back and talk to a product owner and hash out completely how something should work and why it should work in a particular way, only to go back to my desk and crank out the code in a matter of hours."
    C. That is, the Agile approach sucks, but I can't say that in this day and age, is what this blogger who has been recommended to us seems to be saying. 
    D. Anywho, the main point of this rambling blog is the following: "The more and more I write code, the more I learn that understanding the problem is the most critical piece to the equation." [Why do people get paid to do/say the obvious?]
    E. The solution?: 
        1. Make the problem domain easier;
        2. Get better at understanding the problem domain.

## _JavaScript & jQuery_ by Jon Duckett

### Chapter 3: “Object Literals” (pp.100-105)

I. Definitions

    A. "Objects group together a set of variables and functions to create a model of a something you would recognize from the real world."
    B. "In an object, variables and functions take on new names."
        1. "IN an object: variables bcome known as properties."
        2. "In an object: functions become known as methods."
    C. Attributes
        1. "Like variables and named functions, properties and methods have a name and a value. In an object, that name is called a key."
        2. "An object cannot have two keys with the same name. This is because keys are used to access their corresponding values."
        3. "The value of a property can be a string, number, Boolean, array, or even another object. The value of a method is always a function."

II. Name-value pairs

    A. HTML: attribute names and values.
    B. CSS: property names and values.
    C. JavaScript
        1. "Variables have a name and you can assign them a value of a string, number, or Boolean."
        2. "Arrays have a name and a group of values. (Each item in an array is a name/value pair because it has an index number and a value.)"
        3. "Named functions have a name and value that is a set of statements to run if the function is called."
        4. "Objects consist of a set of name/value pairs (but the names are referred to as keys)."

III. Creating an object: leteral notation

    A. "Literal notaiton is the easiest and most popular way to create objects."
    B. "There are several ways to create objects."
    C. "The object is the curly braces and their content.
    D. "The object is stored in a variable called" something. 
    E. "Separate each key from its value using a colon."
    F. "Separate each property [value] and method with a comma (but not after the last value)."

IV. Accessing an object and dot notation

    A. "You access the properties or methods of an object using dot notation." 
    B. "You can also access properties using square brackets."
    C. "The period is known as the member operator. The property or method on its right is a member of the object on its left."
    D. Example: var hotelName = hotel.name; = [on the right side of the variable] this is the object + the property/method name. var roomsFree = hotel.checkAvailability(); 
    E. "You can also access the properties of an object (but not its methods) using square bracket syntax." E.g., var hotelName = hotel['name'];

### Chapter 5: “Document Object Model” (pp.183-242): the DOM

I. Definition of the DOM  

    A. "The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window."
    B. "The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas:"
        1. "Making a model of the HTML page":
            a. "When the browser loads a web page, it creates a model of the page in memory."
            b. "The DOM specifies the way in which the browser should structure this model using a DOM tree."
            c. "The DOM is called an object model because the model (the DOM tree) is made of objects."
            d. "Each object represents a different part of the page loaded in the browser window."
        2. "Accessing and changing the HTML page":
            a. "The DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser."
            b. The DOM = Application Programming Interface (API).
            c. "APls let programs (and scripts) talk to each other." 
            d. "The DOM states what your script can ask the browser about the current page, and how to tell the browser to update what is being shown to the user."
II. The DOM tree, or model of a webpage

    A. Consists of 4 main types of nodes. "Relationships between the document and all of the element nodes are described using the same terms as a family tree: parents, children, siblings, ancestors, and descendants. (Every node is a descendant of the document node.)"
        1. The document node: "At the top of the tree a document node is added; it represents the entire page. . . . It is the starting point for all visits to the DOM tree."
        2. Element nodes: "To access the DOM tree, you start by looking for elements. Once you find the element you want, then you can access its text and attribute nodes if you want to. This is why you start by learning methods that allow you to access element nodes, before learning to access and alter text or attributes."
        3. Attribute nodes: 
            a. "The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree."
            b. "Attribute nodes are not children of the element thar carries them; they are partofthat element."
        4. Text nodes: 
            a. "Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node."
            b. "Text nodes cannot have children."
    B. "Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser."

    ![The DOM Tree](../DOM Tree.jpg)

III. Working with the DOM tree 

    A. Accessing and updating the DOM tree
        1. "Locate the node that represents the element you want to work with."
            a. Select an individual element node.
                i. getElementById(): "Uses the value of an element's id attribute"
                ii. querySelector(): "Uses a CSS selector, and returns the first matching element."
                iii. "You can also select individual elements by traversing from one element to another within the DOM tree" (see point c).
            b. Select multiple elements (nodelists).
                i. getElementsByClassName()
                ii. getElementsByTagName() 
                iii. querySelectorAll(): Uses a CSS selector to select all matching elements.
            c. Traverse between element nodes
                i. parentNode: "Selects the parent of the current element node (which will return just one element)."
                ii. previousSibling / nextSibling: "Selects the previous or next sibling from the DOM tree."
                iii. firstChild / lastChild: "Select the first or last child of the current element."
        2. "Use its text content, child elements, and attributes."