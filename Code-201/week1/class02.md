# Class 02 Reading Notes

## _HTML & CSS_ by Jon Duckett

I. Chapter 2: Text (pp. 40 - 61)

    A. Two typies of markup:
        i. Structural: "the elements that you can use to describe both headings and paragraphs."
        ii. Semantic: "which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on."
    B. Main tags
        i. headings: six levels, <h1> through <h6>, with h1 being reserved for the main heading and the rest for subheadings, meant to be used hierarchically. 
        ii. <p>: "By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs."
        iii. <sup>: "The <sup> element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power such as 22."
        iv. <sub>: "The <sub> element is used to contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20."
    C. Line breaks and horizontal rules (these are empty elements)
        i. <br />: "the browser will automatically show each new paragraph or heading on a new line. But if you wanted to add a line break inside the middle of a paragraph you can use the line break tag."
        ii. <hr />: horizonatal rule.
    D. Semantic markup: "text elements that are not intended to affect the structure of your web pages, but they do add extra information to the pages"
        i. <strong>: bold (by default)
        ii. <em>: italics (by default)
        iii. <blockquote>: "The <blockquote> element is used for longer quotes that take up an entire paragraph. Note how the <p> element is still used inside the <blockquote> element." Don't use this element to introduce indentation; use CSS for that. 
        iv. <q>: IE doesn't recognize it, so it's mostly avoided--is that the case now??--but it puts quotes around text. Both this and the blockquote may have a cite element with a URL assigned to it.
        iv. <abbr>: "If you use an abbreviation or an acronym, then the <abbr> element can be used. A title attribute on the opening tag is used to specify the full term."
        v. <cite>: "When you are referencing a piece of work such as a book, film or research paper, the <cite> element can be used to indicate where the citation is from."
        vi. <dfn>: "The first time you explain some new terminology (perhaps an academic concept or some jargon) in a document, it is known as the defining instance of it."
        vii. <address>: "contain contact details for the author of the page. It can contain a physical address, but it does not have to. For example, it may also contain a phone number or email address."
        viii. <ins> and <del>: "The <ins> element can be used to show content that has been inserted into a document, while the <del> element can show text that has been deleted from it." ins underlines the entry, while del strikes it out.
        ix. <s>: strikethrough. 

II. Chapter 10: Introducing CSS (pp. 226 - 245)

    A. What CSS Does: "CSS allows you to create rules that specify how the content of an element should appear."

    B. How CSS Works

        i. "The key to understanding how CSS works is to imagine that there is an invisible box around every HTML element."
        ii. "CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented."

    C. Rules, Properties, and Values

        i. "A CSS rule contains two parts: a selector and a declaration."
        ii. Ex: p is the selector and font-family: Arial is the declaration.
        iii. "CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon."

    D. Linking CSS to HTML

        i. Internally: style tag nested in the head tag: outdated method. 
        ii. Externally: link tag nested in the head and utilizing the href, type, and rel attributes. 
            a. href: "This specifies the path to the CSS file (which is often placed in a folder called css or styles)."
            b. type: "This attribute specifies the type of document being linked to. The value should be text/css."
            c. "rel: This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file."
        iii. Example
        ---
        <link href="css/styles.css" type="text/css" rel="stylesheet" />
        ---
        iv. Benefits of external over internal linking
            a. "Allows all pages to use the same style rules (rather than repeating them in each page)."
            b. "Keeps the content separate from how the page looks."
            c. "Means you can change the styles used across all pages by altering just one file (rather than each individual page)."
        
    E. CSS Selectors
        i. Case sensitive.
        ii. General types of selectors

    ![General CSS Selectors](Images/General CSS Selectors.jpeg)

    F. "How CSS Rules Cascade"
        
        i. Last Rule: "If the two selectors are identical, the latter of the two will take precedence."
        ii. Specificity: "If one selector is more specific than the others, the more specific rule will take precedence."
        iii. Important: "You can add !important after any property value to indicate that it should be considered more important than other rules that apply to the same element."
        iv. Inheritance: Font-family and color elelments will apply to child elements, while elements like background-color or borders are not inherited. 
        iv. "You can force a lot of properties to inherit values from their parent elements by using inherit for the value of the properties."

---

## _JavaScript & jQuery_ by Jon Duckett

I. Chapter 2: Basic JavaScript Instructions (pages 53 - 84)

    A. Statements
        i. The individual steps of a script; they alwyas end in a semi-colon.
        ii. Each statement should start on a new line.
        iii. The ";" tells the interpreter to move to the next step. 
        iv. Statements may be grouped together in code blocks, surrounded by curly braces {}.
    B. Comments
        i. Comments help make code easier to read.
        ii. It's a good practice using comments to indicate what your code does. 
        iii. // Single-line comments are indicated by two forward slashes before the text
        iv. /* Multi-line comments should be marked off thusly */
    C. Variables
        i. Scripts use variables as temporary containers of information.
        ii. Variables do not store information across browser sessions.
        iii. To declare a variable: `var quantity` is the keyword and name. Use "camelCase" if the variable is more than one word. 
        iv. "Where possible, a variable's name should describe the kind of data [it] holds." 
        v. A variable is undefinded until a value is assigned to it, e.g., quantiy = 3. 
        vi. Six rules for naming a variable:
            a. begins with a letter, dollar sign, or underscore, but _not_ with a number;
            b. contains letters, numbers, dollar sign, and/or underscore, but may not contain a hyphen or a period;
            c. cannot contain keywords, e.g., var, or reserved words, i.e., those reserved for potential future use in JS;
            d. are case sensitive;
            e. uses a name that describes the information stored in it; 
            f. uses camel case. 
    D. Data types include numbers (e.g., 45), strings ('words' or symbols, e.g., '45'), and booleans (true or false). 
    E. Arrays: a special type of variable that stores a list or set of related values, not just one value, e.g., a shopping list. 
        i. Arrays are declared the same way, using var + name
        ii. They are defined using brackets and commas, e.g., colors = ['white', 'black', 'custom']; (this syntax is called an "array literal.") There is an alternative syntax called an "array constructor," which has the var + name set equal to `new Array('white',
                                        'black',
                                        'custom');`
        iii. They may include any type of data type simultaneously. 
        iv. "Values in an array are accessed as if they are [sic] in a number list. . . . [T]he numbering of this list starts at zero (not one)." 

    F. Expressions + Operators
        i. Expresions: "an expression results in a single value"
            a. two types of expressions
                1. assigns a value to a variable: var color = 'beige';
                2. uses two-plus values to return a single value: var area = 3 * 2;

    G. Operators: "allows programmers to create a single value from one or more values"
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

    H. ![Example JS code](../Images/sampleBasicJS.jpeg)

II. Chapter 4: Decisions and Loops (pp. 145 - 162)

    A. Contolling flow (determining which code to run)
        i. Evaluations: analyze values in scripts to determine whether they match expected results.
        ii. Decisions: choose a path to take based on the results of evaluations.
        iii. Loops: repeat a set of steps. 
    B. Decision-making: 
        i. flowcharts help to plan for forks in the road.
        ii. Two components of a decision
            a. "An expression is evaluated, which returns a value," based on which,
            b. "A conditional statement says what to do in a given situation." 
    C. Comparison operators: evaluating conditions, typically return values of true and false
        i. Compare one value with what is expected using a comparison operator and a boolean, 
        ii. Some types of comparison operators
            a. == (is equal to) 
            b. != (is not equal to)
            c. === (is strictly equal to, including data type)
            d. !== (is strictly unequal, including data type)
            e. > (greater than)
            f. < (less than)
            g. >= (greater than or equal to)
            h. <= (less than or equal to)
    D. Logical operators: "allow you to compare the results of more than one comparison operator"
        i. Types
            a. && (logical and): tests more than one condition, e.g., `((2 < 5) && (3 >=2))`
            b. || (logical or): tests at least one condition, e.g., `((2 < 5) || (2 < 1))`
            c. ! (logical not): inverts a single boolean value, e.g., `!(2 < 1) returns true.
        ii. "Logical expressions are evaluated left to right."
    E. If and if...else statements
        A. "The if statement evaluates . . . a condition. If the condition evaluates to true, any statements in the subsequent code block are executed."
        B. "The if...else statement checks a condition. If it resolves to true, the first code block is executed. If the condition resolves to false the second code block is run instead."
