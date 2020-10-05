# Code 201 | Class03 | Reading Notes | 30 September 2020

## _HTML & CSS_ by Jon Duckett

### Chapter 3: Lists (pp. 62 - 73)

I. HTML offers 3 types of lists

    A. Ordered lists: numbered lists.
    B. Unordered lists: bulleted lists.
    C. Definition lists: "made up of a set of terms along with the definitions for each of those terms."

II. Syntax

    A. `<ol>`: ordered list.
    B. `<ul>`: unordered list.
    C. `<li>`: list item.
    D. `<dl>`: definition list, which consists of a term and its definition indented.
        1. `<dt>`: contains the term being defined.
        2. `<dd>`: contains the defintion.
    E. Lists can be nested to create sublists.

### Chapter 13: Boxes (pp. 300 - 329)

I. Box dimensions

    A. Set the width and height dimensions using: 
        1. pixels (px): "Traditionally, pixels have been the most popular method because they allow designers to accurately control their size."
        2. percentages (%): "When you use percentages, the size of the box is relative to the size of the browser window or, if the box is encased within another box, it is a percentage of the size of the containing box."
        3. ems (em): "When you use ems, the size of the box is based on the size of text within it.
    B. Limiting width (min-width, max-width); and height (min-height, max-height)
        1. Useful when your screen sizes may change, ensuring that the content on the page is legible
    C. Overflow: The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
        1. hidden: hides content that doesn't fit.
        2. scroll: "This property adds a scrollbar to the box so that users can scroll to see the missing content."

II. Create borders around boxes

    A. Three properties for controlling how a box looks:
        1. Border: "Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another."
        2. Margin: "Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes."
        3. Padding: "Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents."
    B. Properties
        1. Borders
            a. Width
                i. border-width: value is in pixels, or thin, medium, thick.
                ii. border-top-width, -right-width, -bottom-width, -left-width: controls each side individually.
                iii. shortcut for ii: border-width: 2px 1px 1px 2px (clockwise order: top, right, bottom, left).
            b. Style: border-style
                i. solid
                ii. dotted
                iii. dashed
                iv. double
                v. groove: "appears to be carved into the page"
                vi. ridge: "appears to stick out from the page"
                vii. inset
                viii. outset: "looks like it's coming out of the screen"
                ix. hidden / none
                x. border-top-style, -right-style, -bottom-style, -left-style.
            c. Color: border-color
                i. Use either RGB values, hex codes, HSL, or CSS color names.
                ii. border-top-color, right-color, bottom-color, left-color.
                iii. shortcut for ii: listed clockwise one after the other starting at noon. 
            d. Shorthand for a border's width, style, and color: all in one line; [you need the style at least to make the border show up.]
            e. border-image: "The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces. . . . The property requires three pieces of info":
                i. URL of the image
                ii. where to slice the image
                iii. what to do with the straight edges: stretch, repeat, or round. 
        2. Padding
            a. %, px, or ems; if %, it's of the browser window or containing box
            b. padding-top, -right, -bottom, -left
            c. Shorthand: in line, clockwise from noon. 
        3. Margin: controls the space among boxes.
            a. px, % or ems
            b. Superimposition: "If one box sits on top of another, margins are collapsed , which means the larger of the two margins will be used and the smaller will be disregarded."
            c. margin-top, -right, -bottom, -left
            d. Shorthand: clockwise from noon; or, if list only two values, the first will be the top and bottom, the second will be the right and left. 
    C. Centering content
        1. auto: "If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto."
        2. width: "In order to center a box on the page, you need to set a width for the box (otherwise it will take up the full width of the page)."
    D. Change inline/block: the display property (often used to create nav for a site)
        1. Display: "allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page."
        2. It's values:
            a. inline: "This causes a block-level element to act like an inline element."
            b. block: "This causes an inline element to act like a block-level element."
            c. inline-block: "This causes a block-level element to flow like an inline element, while retaining other features of a block-level element."
            d. none: "hides an element from the page."
    E. Hiding boxes: the visibility property: "The visibility property allows you to hide boxes from users but It leaves a space where the element would have been."
        1. hidden: hides the element
        2. visible: shows the element
        3. "If you do not want a blank space to appear, then you should use the display property with a value of none instead (as covered on the previous page)."
    F. Box shadows: the box-shadow property: "allows you to add a drop shadow around a box."
        1. Horizontal offset: "Negative values position the shadow to the left of the box."
        2. Vertical offset: "Negative values position the shadow to the top of the box."
        3. Blur distance: "If omitted, the shadow is a solid line like a border."
        4. Spread of shadow: "If used, a positive value will cause the shadow to expand in all directions, and a negative value will make it contract."
        4. "The inset keyword can also be used before these values to create an inner-shadow."
    G. Rounded corner: the border-radius property (The value indicates the size of the radius in pixels.)
        1. "You can specify individual values for each corner of a box using" the clockwise method starting at noon.
        2. Or by setting each individually:
            a. border-top-right-radius 
            b. border-bottom-right-radius 
            c. border-bottom-left-radius 
            d. border-top-left-radiusj
        3. Eliptical shapes: 
            a. "To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners."
            b. "You can target just one corner using the individual properties for that corner: border-top-left-radius: 80px 50px;
            c. "There is also a shorthand for targetting all four corners at once; first you specify the four horizontal values, then the four vertical values." 
            d. "You can even create a circle by taking a square box and making the border-radius the same height as the square."

---

## _JavaScript & jQuery_ by Jon Duckett

### Review from Reading 02, Chapter 2: Basic JavaScript Instructions (pp. 70 - 73)

I. Arrays

    A. "An array is a special type of variable. It doesn't just store one value; it stores a list of values."
    B. "You should consider using an array whenever you are working with a list or a set of values that are related to each other."
    C. "Arrays are especially helpful when you do not know how many items a list will contain because, when you create the array, you do not need to specify how many values it will hold."
    D. Creating an array
        1. "You create an array and give it a name just like you would any other variable (using the var keyword followed by the name of the array)."
        2. "The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array."
        3. "Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one)."
II. '[Empty]'

### Chapter 4: Decisions and Loops (starting from switch statements) (pp. 162 - 182)

I. If-else statements

    A. "The if...else statement checks a condition."
        1. "If it resolves to true, the first code block is executed."
        2. If the condition resolves to false, the second code block is run instead."
    B. Switch statements
        1. "A switch statement starts with a variable called the switch value." 
        2. "Each case indicates a possible value for this variable adn the code tha should run if the variable matches that value."
        3. "You have a default option that is run if none of the cases match."
        4. "If a match is found, that code is run; then the break statement stops teh resst of the switch statement running (providing better performance than multiple if statement", which check each condition regardless of whether one has already been met.)
II. Type coercion and weak typing

    A. "If you use a data type JavaScript did not expect, it tries to make sense of the operation rather than report an error."
    B. "JavaScript can convert data types behind the scenes to complete an operation. This is known as type coercion."
    C. "JavaScript is said to use weak typing because the data type for a value can change. Some other languages require that you specify what data type each variable will be. They are said to use strong typing."
    D. "Type coercion can lead to unexpected values in your code (and also cause errors). Therefore, when checking if two values are equal, it is considered better to use strict equals operators ===and ! == rather than == and != as these strict operators check that the value and data types match."
    E. Data types
        1. string = text
        2. number = number
        3. boolean = true or false
        4. null = empty value
        5. undefined = "Variable has been declared but not yet assigned a value"
        5. NaN = "a value that is counted as a number. You may see it when a number is expected, but is not returned, e.g.. ('ten' /2) results in NaN."
    F. "Due to type coercion, every value in JavaScript can be treated as if it were true or false; and this has some interesting side effects."
        1. Falsy values
            a. "Falsy values are treated as if they are fa1se. The table to the left shows a hi ghScore variable with a series of values, all of which are falsy. Falsy values can also be treated as the number 0."
            b. Types;
                i. var highScore = false;
                ii. var highScore = 0;
                iii. var highScore = 10/'score';
                iv. var highScore; "A variable with no value assigned to it"
                v. var highScore = ''; NaN
        2. Truthy values
            a. "Truthy values are treated as if they are true. Almost everything that is not in the falsy table can be treated as if it were true. Truthy values can also be treated as the number 1."
            b. Types:
                i.var highScore = true;
                ii. var highScore = 1; [numbers other than zero];
                iii. var highScore = 'carrot'; [strings with content];
                iv. var highScore = 10/5; [number calculations];
                v. var highScore = 'true'; [true written as a string];
                vi. var highScore = '0';    [zero within a string; because all strings are true, except empty strings];
                vii. var highScore = 'false'; [false written as a string].
III. ![Checking equality and existence](../Truth&False.jpg)

IV. Short circuit values

    A. "Logical operators are processed left to right. They short-circuit (stop) as soon as they have a result - but they return the value that stopped the processing (not necessarily true or fa1se)."
    B. "As soon as a truthy value is found, the remaining options are not checked. Therefore, experienced programmers often:"
        1. "Put the code most likely to return true first in OR operations, and false answers first in AND operations."
        2. "Place the options requiring themostprocessingpowe.r last, just in case another value returns true and they do not need to be run."

V. Loops

    A. They check a condition which, if true, will run a code block; repeated until false. 
    B. Three common types
        1. for: for code that needs to be run a specific number of times.
        2. while: for code that needs to be run an unspecified number of times.
        3. do while: like the while loop, but will run the code block at least once, "even if tihe condition evaluates to false."
    C. Loop counters
        1. "A for loop uses a counter as a condition."
        2. "The condition is made up of three statements":
            a. initialization: var i = 0; = indicates the name of the counter and the starting position.
            b. condition: i < 10 = the limit of the counter.
            c. update: i++ = adding one to the counter after each run of the condition. "It is also possible for loops to count downwards using the decrement operator (--)."
    D. Three important considerations when looping
        1. Keywords: 
            a. break: "This keyword causes the termination of the loop and tells the interpreter to go onto the next statement of code outside of the loop. (You may also see it used in functions.)"
            b. continue: "This keyword tells the interpreter to continue with the current iteration, and then check the condition again. (If it is true, the code runs again.)"
        2. Loops & arrays: 
            a. "Loops are very helpful when dealing with arrays if you want to run the same code for each item in the array."
            b. [empty]
        3. Performance issues:
            a. "It is important to remember that when a browser comes across JavaScript, it will stop doing anything else until it has processed that script."
            b. "If your loop is dealing with only a small number of items, this will not be an issue. If, however, your loop contains a lot of items, it can make the page slower to load." [Maybe this is why JS links are put between the footer and the closing main tag.]
            c. "Any variable you can define outside of the loop and that does not change within the loop should be defined outside of it. If it were declared inside the loop, it would be recalculated every time the loop ran, needlessly using resources."

[<--back](201week1.md)

[<--home-->](../../README.md)
