# Preparatory Readings

## _CSS & HTML_ by Jon Duckett

---

### Introduction (pages 2 - 11)

I. The Structure of the book

    A. HTML
    B. CSS
    C. Practical: advice about making better websites

II. Considering points of accessing the web

    A. Browsers
    B. Web servers
    C. Screen readers
    D. Devices

III. How the web works

    A. "When you connect to the web, you do so via an Internet Service Provider (ISP)."
    B. "Your computer contacts a network of servers called Domain Name System (DNS) servers. These act like phone books; they tell your computer the IP address associated with the requested domain name. An IP address is a number of up to 12 digits separated by periods / full stops. Every device connected to the web has a unique IP address; it is like the phone number for that computer."
    C. "The unique number that the DNS server returns to your computer allows your browser to contact the web server that hosts the website you requested. A web server is a computer that is constantly connected to the web, and is set up especially to send web pages to users."
    D. "The web server then sends the page you requested back to your web browser."

### HTML Chapter 1: “Structure” (pages 12 - 39)

I. Structure

    A. or hierarchy is used, as in a newspaper, to engender understanding. 
    B. HTML describes the structure of web pages. 

II. HTML elements: tags in angled brackets.

    A. Tags act as containers.
    B. They tell the browser something about the info that lies inside them. 
    C. Most often come in pairs of opening and closing tags. 

III. HTML attributes

    A. Provide additional info about the contents of an element. 
    B. "They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign." 

IV. Main HTML elements

    A. <body>: "Everything inside this element is shown inside the main browser window."
    B. <head>: metadata for the browser
        i. Comes before the body;
        ii. Contains info about the page, e.g. <title>, which will display a title on the tab of the page.    

### HTML Chapter 8: “Extra Markup” (pages 176 - 199)

I. The different versions of HTML and how to indicate which version you are using

    A. HTML4: released in 1997
    B. XHTML 1.0: released in 2000: a mix of HTML and XML
    C. HTML5: released in 2000
    D. "Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using." 
    E. "Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. . . . As you will see when you come to look at CSS in the next section, giving an element a unique identity allows you to style it differently than any other instance of the same element on the page."

II. How to add comments to your code: `<!--" comments -->`

III. Global attributes, which are attributes that can be used on any element

    A. "ID attributes can be used to allow JavaScript to work with that particular element."
    B. Class attributes: "Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements as being different from the other elements on the page." 

IV. Elements that are used to group together parts of the page where no other element is suitable

    A. <div>: block-level container
        i. "For example, you might create a <div> element to contain all of the elements for the header of your site (the logo and the navigation), or you might create a <div> element to contain comments from visitors."
        ii. "It can also make it easier to follow your code if you have used <div> elements to hold each section of the page."
        iii. "Since there may be several other elements inside a <div> element, it can be helpful to add a comment after the closing </div> tag."
    B. <span>: the inline equivalent of the div
        i. "Contain a section of text where there is no other suitable element to differentiate it from its surrounding text."
        ii. "Contain a number of inline elements."

V. How to embed a page within a page using iframes

    A. an abbreviation of "inline frame." 
    B. "An iframe is like a little window that has been cut into your page — and in that window you can see another page. "
    C. "One common use of iframes (that you may have seen on various websites) is to embed a Google Map into a page."
    D. "There are a few attributes that you will need to know to use it":
        i. src: "The src attribute specifies the URL of the page to show in the frame."
        ii. height: "The height attribute specifies the height of the iframe in pixels."
        iii. width: "The width attribute specifies the width of the iframe in pixels."
        iv. scrolling: "The scrolling attribute will not be supported in HTML5. In HTML 4 and XHTML, it indicates whether the iframe should have scrollbars or not. This is important if the page inside the iframe is larger than the space you have allowed for it (using the height and width attributes)."
        v. frameborder: "The frameborder attribute will not be supported in HTML5. In HTML 4 and XHTML, it indicates whether the frame should have a border or not."
        vi. seamless: "In HTML5, a new attribute called seamless can be applied to an iframe where scrollbars are not desired. The seamless attribute (like some other new HTML5 attributes) does not need a value, but you will often see authors give it a value of seamless. Older browsers do not support the seamless attribute."

VI. How to add information about the web page using the `<meta>` element

    A. "The <meta> element lives inside the <head> element and contains information about that web page."
    B. "It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can be set to expire.)"
    C. Empty = no closing tag.
    D. "The most common attributes are the name and content attributes, which tend to be used together. These attributes specify properties of the entire page. The value of the name attribute is the property you are setting, and the value of the content attribute is the value that you want to give to this property."
    E. "The value of the name attribute can be anything you want it to be. Some defined values for this attribute that are commonly used are:"
        i. description: "This contains a description of the page. This description is commonly used by search engines to understand what the page is about and should be a maximum of 155 characters. Sometimes it is also displayed in search engine results."
        ii. keywords: "This contains a list of comma- separated words that a user might search on to find the page. In practice, this no longer has any noticeable effect on how search engines index your site."
        iii. robots: "This indicates whether search engines should add this page to their search results or not. A value of noindex can be used if this page should not be added. A value of nofollow can be used if search engines should add this page in their results but not any pages that it links to."
    F. author: defines the author of the page.
    G. pragma: prevents the browser from caching the page. 
    H. expires: "Because browsers often cache the content of a page, the expires option can be usedto indicate when the page should expire (and no longer be cached). Note that the date must be specified in the format shown." `["Fri, 04 Apr 2014 23:59:59 GMT"]`

VII. Adding characters such as angled brackets and copyright symbols

    A. Use "escape" characters (aka escape codes or entity references) before and after. 
    B. Eg: left angle bracket < = &lt; or &#60.
    C. & = &amp; or &#38. 
    D. Copyright symbol = &copy; or &#169.
    E. "When using escape characters, it is important to check the page in your browser to ensure that the correct symbol shows up. This is because some fonts do not support all of these characters and you might therefore need to specify a different font for these characters in your CSS code."

VIII. BLock and inline elements

    A. Block: always come with a hard return built in. E.g., headers, paragraph, ul and li.
    B. Inline: no built-in hard return. E.g., anchor, font styling elements, img. 

### HTML Chapter 17: “HTML5 Layout” (pages 428 - 451)

I. A little context

    A. "For a long time, web page authors used `<div>` elements to group together related elements on the page (such as the elements that form a header, an article, footer or sidebar). Authors used class or id attributes to indicate the role of the `<div>` element in the structure of the page."
    B. "HTML5 introduces a new set of elements that allow you to divide up the parts of a page. The names of these elements indicate the kind of content you will find in them."
    C. Instead of div id="header", for example, you have `<header>` as its own element. 
    D. "The point of creating these new elements is so that web page authors can use them to help describe the structure of the page."

II. Elements

    A. <header>; <footer>; "Each individual <article> and <section> element can also have its own <header> and <footer> elements to hold the header or footer information for that section within the page."
    B. <nav>: "used to contain the major navigational blocks on the site such as the primary site navigation"; often placed in the header.
    C. <article>: "The <article> element acts as a container for any section of a page that could stand alone and potentially be syndicated. This could be an individual article or blog entry, a comment or forum post, or any other independent piece of content."
    D. <aside>: "has two purposes, depending on whether it is inside an <article> element or not":
        i. inside: "it should contain information that is related to the article but not essential to its overall meaning. For example, a pullquote or glossary might be considered as an aside to the article it relates to."
        ii. outside: "it acts as a container for content that is related to the entire page. For example, it might contain links to other sections of the site, a list of recent posts, a search box, or recent tweets by the author."
    E. <section>: "groups related content together, and typically each section would have its own heading. . . . Because the <section> element groups related items together, it may contain several distinct <article> elements that have a common theme or purpose."
    F. <hgroup>: heading groups "The purpose of the <hgroup> element is to group together a set of one or more <h1> through <h6> elements so that they are treated as one single heading."
    G. <figure>: "It can be used to contain any content that is referenced from the main flow of an article (not just images)." E.g., for images, video, graphs, diagrams, code samples, supporting text. "The <figure> element should also contain a <figcaption> element which provides a text decription for the content of the <figure> element."
    H. <div>: "you should not be using these new elements that you have just met for purposes other than those explicitly stated." In which cases, you'll use a div. 

### HTML Chapter 18: “Process & Design” (pages 452 - 475)

I. Audience: the foremost principle for guiding your design choices.

    A. Age range and gender appeal
    B. Location and language
    c. Levels of income and education
    D. Family and employment status
    E. Computer saavy and usage, including preferred devices
    F. If a company, its size, the role(s) of its representatives visiting the site, whether they're visiting for the company's or its clients' sake, and its budget

II. Motives: why your site's visitors come.

    A. Motivations
        i. General entertainment or a specific aim?
        ii. If an aim: personal or professional?
        iii. Is the visit essential or optional? 
    B. Goals
        i. General research or a specific aim?
        ii. Known product or needs an introduction?
        iii. Looking for time-sensitive information? 
        iv. Looking for info on a product or service to help them decide whether to purchase? 
        v. Looking for contact information? If so, in person or remotely? 

III. Steps to wire-framing your site.

    A. Who: List the demographics of your audience.
    B. Why: List the main reasons people will visit your site.
    C. What: List the information your visitors will need. 
    D. How (often): Determine whether the site needs frequent updating based on the frequency a discrete user may visit.

IV. Site Maps: A diagram of the pages used to structure the site

    A. Card sorting: "placing each piece of information that a visitor might need to know on a separate piece of paper and then organizing the related information into groups."
    B. "The groups of information are then turned into the diagram that is known as the site map."
    C. "If the site is large and is compartmentalized into sections, each section might require its own section homepage to link to all of the information within it."

V. Wireframes: "a simple sketch of the key information that needs to go on each page of a site."

    A. "By creating a wireframe you can ensure that all of the information that needs to be on a page is included."
    B. "You should not include the color scheme, font choices, backgrounds or images for the website in the wireframe."

VI. Design: "Organizing and prioritizing information on a page helps users understand its importance and what order to read it in."

    A. Content
    B. Prioritizing using visual hierarchy: "By making parts of the page look distinct from surrounding content, designers draw attention to (or away from) those items."
        i. Size
        ii. Color
        iii. Style
    C. Organizing by grouping: "Grouping together related content into blocks or chunks makes the page look simpler (and easier to understand)."
        i. Proximity
        ii. Closure: "A real or imaginary box can be formed around elements due to their proximity and alignment."
        iii. Continuance: "When elements are placed in a line or a curve then they are perceived to be more related than those that are not following the same direction."
        iv. White space: "Placing related items closer together and leaving a bigger gap between unrelated items."
        v. Background color: "A background color placed behind related items to emphasize their connection."
        vi. Borders
    D. Other defining elements
        i. Consistency
        ii. Headings

VII. Navigations

    A. Concise: "the navigation should be quick and easy to read."
    B. Clear: "Users should be able to predict the kind of information that they will find on the page before clicking on the link."
    C. Selective: "The primary navigation should only reflect the sections or content of the site."
    D. Context: "Good navigation provides context. It lets the user know where they are in the website at that moment."
    E. Interactivity: "Each link should be big enough to click on and the appearance of the link should change when the user hovers over each item or clicks on it."
    F. Consistency: "Although secondary navigation will change from page to page, it is best to keep the primary navigation exactly the same."

---

## _JavaScript & jQuery_ by Jon Duckett

---

### Introduction

I. I. Pages 1 - 12: Intro

    A. "This book explains how JavaScript can be used in browsers to make websites more interactive, interesting, and user-friendly. You will also learn about jQuery because it makes writing JavaScript a lot easier."

    B. JS makes web pages more interactive by accessing and modifying the content of the webpage while in use. 
        i. **Accessing* content: "You can use JavaScript to select any element, attribute, or text from an HTML "
        ii. **Modifying** content: "You can use JavaScript to add elements, attributes, and text to the page, or remove them."
        iii. **Program** rules: "You can specify a set of steps for the browser to follow (like a recipe), which allows it to access or change the content of a page."
        iv. **Reacting** to events: "You can specify that a script should run when a specific event has occurred.

### Chapter 1: The ABC of Programming (pages 11 - 52)

I. "A script is a series of instructions that a computer can follow to achieve a goal" like:
    A. Receipes
    B. Handbooks
    C. Manuals

II. Writing a script: "To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it."
    A. Define the goal
    B. Design the script: "To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle."
    C. Code each step

III. Desigining a script
    A. Tasks: The goal defines the individual **tasks** needed to achieve it, e.g., tidy a room
    B. Steps: each task may be reduced to a sequence of steps, which in turn may be translated into lines of code, e.g., the steps required to tidy a room.

IV. Code
    A. vocabulary: "the words that computers understand"
    B. syntax: "How you put those words together"

V. Desinging a goal
    a. Define the goal
    b. List the steps required to acheive it
    c. Sketch out the tasks in a flowchart

[<--back](../201week1.md)

[<--home-->](../../README.md)
