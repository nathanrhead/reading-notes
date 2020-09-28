# Notes on Programming with JS: Reading 07

## _JavaScript and JQuery_ by Jon Duckett

I. Pages 1 - 12: Intro

    A. "This book explains how JavaScript can be used in browsers to make websites more interactive, interesting, and user-friendly. You will also learn about jQuery because it makes writing JavaScript a lot easier."

    B. JS makes web pages more interactive by accessing and modifying the content of the webpage while in use. 
        i. **Accessing* content: "You can use JavaScript to select any element, attribute, or text from an HTML "
        ii. **Modifying** content: "You can use JavaScript to add elements, attributes, and text to the page, or remove them."
        iii. **Program** rules: "You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page."
        iv. **Reacting** to events: "You can specify that a script should run when a specific event has occurred.

II. Pages 13 - 24, Chapter 1: The ABCs of Programming

    A. "A script is a series of instructions that a computer can follow to achieve a goal" like:
        i. Receipes
        ii. Handbooks
        iii. Manuals
    
    B. Writing a script: "To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it."
        i. Define the goal
        ii. Design the script: "To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle."
        iii. Code each step

    C. Desigining a script
        i. Tasks: The goal defines the individual **tasks** needed to achieve it, e.g., tidy a room
        ii. Steps: each task may be reduced to a sequence of steps, which in turn may be translated into lines of code, e.g., the steps required to tidy a room

    D. Code
        i. vocabulary: "the words that computers understand"
        ii. syntax: "How you put those words together"

    E. Desinging a goal
        i. Define the goal
        ii. List the steps required to acheive it
        iii. Sketch out the tasks in a flowchart

III. Pages 74 - 79: Expressions + Operators

    A. Expresions: "an expression results in a single value"
        i. two types of expressions
            a. assigns a value to a variable: var color = 'beige';
            b. uses two-plus values to return a single value: var area = 3 * 2;

    B. Operators: "allows programmers to create a single value from one or more values"
        i. Some types of operators
            a. Assignment: color = 
            b. Arithmetic: area = 
            c. String (combines two strings): greeting = "Hi" + "Molly";
            d. Comparison (returns true or false): buy = 3 > 5; (false)
            e. Logical (combine expressions): Buy = (5>3) && (2 < 4); (true)
        ii. Arithmetic operators
            a. addition +
            b. substraction -
            c. Division /
            d. Multiplication *
            e. Increment ++ : Adds one to the current number
            f. decrement -- : Subtracts one from the current number
            g. Modulus % : divides two values and returns the remainder
        iii. Order of execution
            a. Multiplication and division, then;
            b. Addition and subtraction. 
            c. To change the priority, use parentheses around the first calculation. 
        iv. String operator is + and is used to join two strings. 

IV. Pages 88 - 94: Functions

    A. Purpose: "Functions let you group a series of statements together to perform a specific task."
    
    B. Utility: 
        i. "Grouping together the statements that are required to answer a question or perform a task helps organize your code."
        ii. "Furthermore, the statements in a function are not always executed whenapageloads,sofunctions also offer a way to store the steps needed to achieve a task. The script can then ask the function to perform all of those steps as and when they are required. If you are going to ask the function to perform its task later, you need to give your function a name. That name should describe the task it is performing."
        iii. "Some functions need to be provided with information in order to achieve a given task. For example, a function to calculate the area of a box would need to know its width and height. Pieces of information passed to a function are known as parameters."
        iv. "You can also have anonymous functions. They do not have a name, so they cannot be called. Instead, they are executed as soon as the interpreter comes across them."
    
    C. Declaring and Calling a Function
        i. Declaring a function: "To create a function, you give it a name and then write the statements needed to achieve its task inside curly braces."
            a. eg. 
                function say Hello() {
                    document.write('Hello!');
                }
            b. "Functions store code required to perform a specific task, and the script can ask the function to perform that task whenever needed.
        ii. Calling a function: "Having declared the function, you can then execute all of the statements between its curly braces with just one line of code." 
            a. To run the code in the function, you use the function name followed by parenteses: sayHello();
            B. The same function may be called as often as needed within the same JS file. 
        iii. In cases when a function requires informaiton to run its task, include parameters in the declaration; the parameters act as variables. 

            a. Ex: function getArea (width, height) {
                return width * height; 
            }

            b. Each time you call this function, the values of the parameters may be different. 
        iv. Calling functions with parameters
            a. Specify the values that the function should use in the parentheses. These values are called arguments and may be provided as values or variables. 
            b. Ex.: getArea(3, 5); or getArea(wallWidth, wallHeight);

[<--home-->](../README.md)
