# About HTML: the Duckett Readings

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
    D. How `(often)`: Determine whether the site needs frequent updating based on the frequency a discrete user may visit.

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

VII. HTML5 Layout

    A. "HTML5 introduces a new set of elements that allow you to divide up the parts of a page `(instead of using div for them)`."
        i. Header and footer
        ii. nav: "The nav element is used to contain the major navigational blocks on the site such as the primary site navigation."
        iii. article: "The `<article>` element acts as a container for any section of a page that could stand alone and potentially be syndicated."
        iv. aside: 
            a. "When the `<aside>` element is used inside an `<article>` element, it should contain information that is related to the article but not essential to its overall meaning."
            b. "When the `<aside>` element is used outside of an `<article>` element, it acts as a container for content that is related to the entire page."
        v. Sections: "The `<section>` element groups related content together, and typically each section would have its own heading."
    B. Div: "the `<div>` element will remain an important way to group together related elements, because you should not be using these new elements that you have just met for purposes other than those explicitly stated."

VIII. Extra Markup

    A. Different versions of HTML
        i. HTML4: 1997
        ii. XHTML 1.0: 2000
        iii. HTML4: 2000
    B. Adding comments: `<!-- comment goes here -->`
    C. Global attributes: attributes that can be used on any element, including the class and id attributes.
    D. Elements that are used to group together parts of a page where no other element is suitable.
        i. block elements: come with a hard return hardcoded in, e.g., headers, paragraphs, unordered lists, and list items.
        ii. inline elements: no hard return, e.g., anchors, bolding, italics, and images. 
        iii. div: "The `<div>` element allows you to group a set of elements together in one block-level box."
        iv. span: "The `<span>` element acts like an inline equivalent of the `<div>` element. It is used to either:
            a. "contain a section of text where there is no other suitable element to differentiate it from its surrounding text, or;
            b. contain a number of inline elements.
        E. Embedding using iframes: "An iframe is like a little window that has been cut into your page — and in that window you can see another page. The term iframe is an abbreviation of inline frame." E.g., google map on a web site. 
        F. Using the `<meta>` element
            i. "The `<meta>` element lives inside the <head> element and contains information about that web page."
            ii. "It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can be set to expire.)"
    G. Adding special symbols: "There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.) Therefore, if you want these characters to appear on your page you need to use what are termed "escape" characters."
        i. left-angeled bracket: &lt; or &#60
        ii. Ampersand: &amp; or &#38
        iii. Copyright symbol: &copy; or &#169

<a href="index.html"><button type="button">Home</button></a>




