# Code 201 | Audio, Video, Images

## Class 11 Reading Notes

### Chapter 16: “Images” (pp. 406 - 427), from _HTML & CSS_ by Jon Duckett

I. Controling size: "You can control the size of an image using the width and height properties in CSS, just like you can for any other box."

  A. "Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download."

  B. "Whenever you use consistently sized images across a site, you can use CSS to control the dimensions of the images, instead of putting the dimensions in the HTML."

  C. "You need to determine the sizes of images that will be used commonly throughout the site, then give each size a name," e.g., small, medium, and large. "Where the `<img>` elements appear in the HTML, rather than using width and height attributes you can use these names as values for the class attribute."

II. Aligning images: "Rather than using the `<img>` element's align attribute, web page authors are increasingly using the float property to align images" in one of two ways:

  A. "The float property is added to the class that was created to represent the size of the image";

  B. "New classes are created with names such as align-left or align-right to align the images to the left or right of the page. These class names are used in addition to classes that indicate the size of the image."

III. Centering images: "By default, images are inline elements. This means that they flow within the surrounding text. In order to center an image, it should be turned into a block- level element using the display property with a value of block," then use one of the following two ways to center it:

  A. "On the containing element, you can use the text-align property with a value of center."

  B. "On the image itself, you can use the use the margin property and set the values of the left and right margins to auto."

IV. Background images

  A. "The background-image property allows you to place an image behind any HTML element. This could be the entire page or just part of the page. By default, a background image will repeat to fill the entire box." (background-image: url("images/pattern.gif");})

  B. Repeating images

    1. background-repeat: 

      a. repeat: "The background image is repeated both horizontally and vertically (the default way it is shown if the background- repeat property isn't used)."
      b. repeat-x: "The image is repeated horizontally only."
      c. repeat-y: "The image is repeated vertically only."
      d. no-repeat: "The image is only shown once."

    2. background-attachment: "The background-attachment property specifies whether a background image should stay in one position or move as the user scrolls up and down the page."

      a. fixed: "The background image stays in the same position on the page."
      b. scroll: "The background image moves up and down as the user scrolls up and down the page."

  C. Background position (background-position): "When an image is not being repeated, you can use the background-position property to specify where in the browser window the background image should be placed."

    1. "This property usually has a pair of values. The first represents the horizontal position and the second represents the vertical." E.g., left top, left center, right bottom, etc. "If you only specify one value, the second value will default to center."

    2. "You can also use a pair of pixels or percentages. These represent the distance from the top left corner of the browser window (or containing box). The top left corner is equal to 0% 0%. The example shown, with values of 50% 50%, centers the image horizontally and vertically."

    3. "Using CSS, it is possible to create a link or button that changes to a second style when a user moves their mouse over it (known as a rollover) and a third style when they click on it.This is achieved by setting a background image for the link or button that has three different styles of the same button (but only allows enough space to show one of them at a time).

  D. Shorthand

    1. "The background property acts like a shorthand for all of the other background properties."

    2. "The properties must be specified in the following order, but you can miss any value if you do not want to specify it":

      a. background-color;
      b. background-image;
      c. background-repeat;
      d. background-attachment;
      e. background-position.

V. Gradients: background-image: "The gradient is created using the background-image property."

VI. Contrast of background images: "If you want to overlay text on a background image, the image must be low contrast in order for the text to be legible."

### Chapter 19: “Practical Information” (pp. 476 - 492), from _HTML & CSS_ by Jon Duckett

I. Search Engine Optimization (SEO)

  A. The basics

    1. Definition: 
    
      a. "Search engine optimization (or SEO) is the practice of trying to help your site appear nearer the top of search engine results when people look for the topics that your website covers."
      b. "At the heart of SEO is the idea of working out which terms people are likely to enter into a search engine to find your site and then using these terms in the right places on your site to increase the chances that search engines will show a link to your site in their results."
    
    2. How the ratings work: "search engines do not only look at what appears on your site. They also consider how many sites linkto you (and how relevant those links are)."

  B. The two techniques to determine relevance:

    1. On-page: "On-page techniques are the methods you can use on your web pages to improve their rating in search engines."

      a. "The main component of this is looking at keywords that people are likely to enter into a search engine if they wanted to find your site, and then including these in the text and HTML code for your site."
      b. "Search engines rely very heavily on the text that is in your pages so it is important that the terms people are going to search for are in text."
      c. "There are seven essential places where you want your keywords to appear."

        i. title of the page
        ii. URL
        iii. Headings (<hn> element)
        iv. text: "Where possible, it helps to repeat the keywords in the main body of the text at least 2-3 times. Do not, however, over-use these terms, because the text must be easy for a human to read."
        v. link text: use keywords instead of "click here." 
        vi. Image alt text
        vii. Page descriptions: lives inside the head; specified using the meta tag. "These are not shown in the browser window but they may be displayed in the results pages of search engines."

    2. Off-page: "Search engines help determine how to rank your site by looking at the number of other sites that link to yours."

      a. "They are particularly interested in sites whose content is related to yours."
      b. "Search engines also look at the words between the opening <a> tag and closing </a> tag in the link. If the text in the link contains keywords (rather than just click here or your website address) it may be considered more relevant."
      c. "The words that appear in links to your site should also appear in the text of the page that the site links to."

  C. Identifying keywords

    1. Brainstorm

      a. "List down the words that someone might type into Google to find your site. Be sure to include the various topics, products or services your site is about."
      B. Don't neglect phrases.

    2. Organize

      a. "Group the keywords into separate lists for the different sections or categories of your website."
      b. "On a large site you may break this up further into sub-categories."

    3. Research

      a. "There are several tools that let you enter your keywords and then they will suggest additional keywords you might like to consider, such as: adwords.google.co.uk/ select/KeywordToolExternal (when using this tool, select the "exact match" option rather than "broad match"); www.wordtracker.com www; keyworddiscovery.com.
      b. "Once these tools have suggested additional keywords, add the relevant options to your lists."

    4. Compare

      a. "It is very unlikely that your site will appear at the top of the search results for every keyword. This is especially true for topics where there is a lot of competition."
      b. "Some of the keyword research sites can tell you how many people have searched for a specific keyword to help you know how much competition those terms have."
      c. "You can also use Google's advanced search feature to just search the titles of web pages. This will help you to determine how many sites have that keyword in the title of their pages."
      

    5. Refine

      a. Pick the keywords and phrases that are most relevant to your site.
      b. "If there is a phrase that is very relevant but you find there is a lot of competition, you should still use it."
      c. "If the information or service you offer on your website is location specific, then you will often find that incorporating your location into your keyword list will help people find you."

    6. Map

      a. "Pick 3-5 keywords or phrases that map to each page of your website and use these as the keywords for each page."
      b. "You should not need to repeat the same keywords on all of the pages. It is also likely that, as you move further away from the homepage into the sections of the site, the keywords will become more specific to the individual topic dealt with on each page."

II. Analyzing your visitors using Google analytics

  A. Signing up: google.com/analytics; "The site will give you a piece of tracking code which you need to put on every page of your site."
  B. How it works: "Every time someone loads a page of your site, the tracking code sends data to the Google servers where it is stored. Google then provides a web- based interface that allows you to see how visitors use your site."
  C. The tracking code: "A tracking code is provided by Google Analytics for each website you are tracking. It should appear just before the closing </head> tag. The code does not alter the appearance of your web pages."
  D. Numbers of visitors

    1. Visits: "This is the number of times people have come to your site. If someone is inactive on your site for 30 minutes and then looks at another page on your site, it will be counted as a new visit."
    2. Unique visits: "This is the total number of people who have visited your site over the specified period. The number of unique visits will be lower than the number of visits if people have been returning to your site more than once in the defined period."
    3. Page views: "The total number of pages all visitors have viewed on your site."
    4. Pages per visit: "The average number of pages each visitor has looked at on your site per visit."
    5. Average time on site: per visit.
    6. Date selector: "Using the date selector in the top right hand corner of the site, you can change the period of time the reports display."
    7. Export: to other apps like Excel.

  E. What they're viewing

    1. Pages: which get visited the most in term of visitors and time visited.
    2. Landing pages: sometimes visitors don't enter your site from the home page.
    3. Top exit pages: the pages most typically viewe last.
    4. Bounce rate: "This shows the number of people who left on the same page that they arrived on. A high bounce rate suggests that the content is not what they were looking for or that the page did not sufficiently encourage them to look around the rest of the site." A bounce is defined as:

      a. "Clicked a link to another site";
      b. "Clicked on an advertisement";
      c. "Entered a new URL";
      d. "Used the "back" button";
      e. "Closed the browser".

  F. Visitor's provenance

    1. References: "This shows the sites that have linked to you and the number of people who have come via those sites."
    2. Direct: "This shows which page a user arrived on if they did not come via a link on another site. They might have typed the URL into their browser, used a browser bookmark, or clicked a link in an email, PDF, or Word document."
    3. "This shows the terms users entered into a search engine to find your site."

  G. Advanced features: ""We have only scratched the surface of what you can find out about your visitors from Google Analytics. Their help files tell you many more of the advanced features. If you run an online shop, it is well worth looking at their e-commerce tracking, which adds information about products sold, average basket size and much more. You can also set up goals where you specify the paths you want people to take, and then see how far they get through those paths, which is especially useful when gathering data from users."

III. Domain names and hosting

  A. Domain names: "Your domain name is your web address (e.g. google.com or bbc. co.uk). There are many websites that allow you to register domain names. Usually you will have to pay an annual fee to keep that domain name."
  B. "With the exception of some very large sites, most websites live on web servers run by web hosting companies. This is usually far cheaper and more reliable than trying to run your own web servers."
  C. Email accounts: "Most hosting companies will provide email servers with their web hosting packages. You will want to check the size of mailbox you are allowed and the number of mailboxes you can use."
  D. Server-side languages and databases: "If you are using a content management system, it will likely use a server-side programming language and a database (such as PHP with a MySQL database, or ASP.Net with a SQL Server database). Be sure to check that your hosting company supports the technologies your software needs to run."

IV. FTP & third-party tools

  A. File Transfer Protocol: "As the name suggests, [FTP] allows you to transfer files across the Internet from your computer to the web server hosting your site."
  B. "Some hosting companies offer tools to upload files to their servers using a web browser, but it is more common to use an FTP program as they are faster at transmitting files."
  C. "There are a wide variety of sites that offer services commonly created by web developers (to save you having to build them yourself)."

### Chapter 9: Flash, Video, & Audio (pp. 200 - 205 only)

I. Introduction: "Flash is a very popular technology used to add animations, video, and audio to websites. This chapter begins by looking at how to use it in your web pages."

II. Because flash is (a) a security risk, (b) a resource hog, and (b) an unreliable platform, devs stopped using it and, as of 31 December 2020, Adobe will discontinue supporting it.

III. Why it's going away, according to Duckett

  A. "In 2005-6, a set of JavaScript libraries were launched (including Prototype, script.aculo.us, and JQuery) which made it easier for people to create animated effects using JavaScript."

  B. "When Apple launched the iPhone in 2007 and later the the iPad in 2010, they took the decision not to support Flash."

  C. "There have been laws introduced to ensure that websites are usable by those with visual or physical impairments — and Flash has been criticized because Flash content does not always meet accessibility requirements."

  D. "In 2008, browsers started to support HTML5 `<video>` and `<audio>` tags."

[<--back](201week3.md)

[<--home-->](../../README.md)
