# Notes on Operators and Loops: Reading 08

## From _JavaScript and jQuery_ by Jon Duckett

I. Comparison and Logical Operators (pages 150, 151, 156, 157)

    A. Comparison Operators
        i. Evaluating conditions
            a. You can evaluate a sitatuion by comparing two values, with the result being true or false. 
            b. operators
                i. == is equal to
                ii. != is not equalt to
                iii. === strictly equal to (both value and data type)
                iv. > greater than and <less than and >= and <=
        ii. Sturcturing comparison operators
            a. There are usually one operator and two operands
            b. The operands go on either side of the operator and may be values or variables
            c. Ex: (score >= pass)

    B Logical Operators
        i. While comparison operators typically answer true or false, logical operators "allow you to compare the results of more than one comparison operator. 
        ii. Ex: ((5 < 2) && (2 >= 3)) and evaluates to false. 
        iii. Types of logical operators
            a. && = logical and: tests more than one condition (as above)
            b. || = logical or: tests at least one condition, e.g., ((2 < 5) || (2 < 1)) returns true, because one of the conditions is met
            c. ! = logical not: "This operator takes a single boolean value and inverts it," e.g., !(2 < 1) returns true
            d. Logical expressions are evaluated from left to right.

II. *for* and *while* loops (pages 170 - 173, 176)

    A. Defining loops: they check a condition, which, if true, will trigger a code block to run; the condition will continue to be checked and trigger the code block as long as it returns a value of true; false will cease the running of the loop. 
    
    B. Three types of common loops
        i. for: to run code a specific number of times. The condition here is typically a counter with the number of times the loop should run. 
        ii. while: used for an indefinite number of times; the condition may be something besides a counter; teh code will loop as long as the condition is true. 
        iii. do while: "the do . . . while loop . . . will always run the statements inside the curly braces at least once, even if the condition evaluates to false." 

    C. Example of a for loop that counts to 9: 

        for (var i = 0; i <10; i++) {
            document.write(i);
        }

    D. Loop counters 
        i. a for loop uses a counter as a condition.
        ii. the condition is made up of three statements:
            a. Initialization: create a variable and set it to zero: var i = 0; 
            b. Condition: the loop should run until the counter reaches a certain number: i < 10; means the loop will run 10 times before stopping (0-9)
            c. Update: adds one to the counter after each run: i++ or i + 1. 
        
    E. Using while loops: an example of a the 5 timestable through 9.

        var i = 1;      //sets the counter to 1
        var msg = '';   //the message

        while  (i < 10) {
            msg += i + ' x 5 = ' + (i * 5) + '<br />';
            i++;
        }

[<--home-->](/README.md)
