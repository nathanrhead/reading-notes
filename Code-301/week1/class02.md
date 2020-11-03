# Code 301 | jQuery, Events, and the DOM; Pair Programming

## Class 02 Reading Notes

## _JavaScript & jQuery_ by Jon Duckett

### "jQuery", excerpt from chapter 7 (pp. 293 - 301)

I. jQuery: Introduction: a simpler way to write JS, it is a JS file that you include in your web pages

  A. Select Elements: "It is simpler to access elements using jQuery's CSS-style selectors than it is using DOM queries. The selectors are also more powerful and flexible."

  B. Perform Task: "jQuery's methods let you update the DOM tree, animate elements into and out of view, and loop through a set of elements, all in one line of code."

  C. Handle Events: "jQuery includes methods that allow you to attach event listeners to selected elements without having to write any tailback code to support older browsers."

III. How it works: jQuery creates an object called jQuery which holds references to the elements you want.

  A. jQuery() is typically written as $()

  B. CSS-style selector: $('li.hot') = finds all "li"s with a class of hot.

  C. jQuery selectors perofrm tasks similar to those of the traditional DOM, but using simpler syntax.

  D. The jQuery object may be stored in a variable, as with DOM nodes.

  E. jQuery methods and properties may be used to manipulate the selected DOM nodes.

III. jQuery Methods and differences with the DOM

  A. A matched set, or jQuery selection: jQuery object + method, e.g., $('li.hot').addClass('complete');: this adds the class "complete" to "li"s with class "hot".

  B. Differences with the DOM

    1. It works across all browsers without fallback code.

    2. Selecting elements is simpler and more accurate.

    3. Event handling uses one method that works on all major browsers.

    4. Methods affect all selected elements without looping.

    5. You may apply multiple methods to a selection.

### "jQuery", excerpt from chapter 7 (pp. 306 - 331)

I. A matched set, or jQuery selection

  A. Single element: when a selector returns one element, which is assigned an index of 0.

  B. Mulitple elements: when a selector returns more than one element, all of which are assigned an index number.

II. Methods that get and set data

  A. Get information: a jQuery selection with multiple elements will only return the content of the first element. To retrieve info from subsequent elements, use traverse or filter or write a more specific selector; or use the .each() method.

  B. Set information: will update the info of each element in a selection. To update the content of only one element, use traverse, filter, or write a more specific selector.

III. Caching jQuery selections in variables

  A. To save resources, instead of creating the same jQuery object again, use a variable to store a reference to it.

  B. Example

    1. Select the element and create the jQuery object: $('li');

    2. Create a variable to store a reference to this object: $listItems = $('li');

IV. Implicit iteration = no more looping.

  A. When a selector returns mulitple elements, one method may be used to update all of them without looping.

  B. To retrieve info from a series of elements, use the .each() method instead of a loop.

V. Chaining

  A. List several methods at a time using dot notations, e.g., $('li[id!="one"]').hide().delay(500).fadeIn(1400);

  B. It's fine to place each method on a new line for legibility.

  C. Methods that retrieve info from the DOM cannot be chained; and if one method doesn't work in a chain, the rest won't, either.

VI. Checking for readiness: use A or B to trigger your jQuery script.

  A. the long way: $(document).ready(function) { your script };

  B. the short way: $(function() { your script });

  C. Other ready functions:

    1. .load() = use this when your script relies on assets having loaded. 

    2. .ready() = checks whether the browser supports DOMContentLoaded. 

    3. Or, just put your script at the bottom before the closing body tag. 

VII. Using .html() and .text() to get and set information

  A. .html() = retrieves info only from the first element in a selection with multiple; returns the html tags as well as text.

  B. .text() = retrieves info from all elements in a selection; only returns the text, not the html tags.



### "jQuery", excerpt from chapter 7 (pp. 354 - 357)

### ["Six Reasons for Pair Programming"](https://www.codefellows.org/blog/6-reasons-for-pair-programming/){:target="_blank" rel="noopener"}

[<--back](301week1.md)

[<--home-->](../../README.md)
