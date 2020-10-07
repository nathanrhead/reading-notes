
# Chapter 15: Layout (pp. 358 - 404) from _HTML & CSS_ by Jon Duckett

I. Positioning elements using normal flow, relative positioning, absolute positioning and floats.

  A. Block-level vs. inline elements

    1. "Block-level boxes start on a new line and act as the main building blocks of any layout."
    2. "Inline boxes flow between surrounding text."
  
  B. Containing elements

    1. "If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element."
    2. "It is common to group a number of elements together inside a <div> (or other block-level) element."
    3. "The containing element is always the direct parent of that element."
  
  C. Positioning elements

    1. Normal flow: default behavior, with all block-level elements lining up one atop another. No need to indicate a position for normal, but were you to, you'd write "position: static;". 
    2. Relative positioning: 
      a. "This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed [normally]. . . . You then use the offset properties (top or bottom and left or right) to indicate how far to move the element from where it would have been in normal flow."
      b. "This does not affect the position of surrounding elements; they stay in the position they would be in in normal flow."
    3. Absolute positioning: 
      a. "This positions the element in relation to its containing element."
      b. "It is taken out of normal flow, meaning that it does not affect the position of any surrounding elements (as they simply ignore the space it would have taken up)."
      c. "Absolutely positioned elements move as users scroll up and down the page."
      d. "The box offset properties (top or bottom and left or right) specify where the element should appear in relation to its containing element."
    4. Fixed positioning: "This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element." Also uses the offset properties of left, right, top, and bottom.
    5. Floating elements: "Floating an element allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow."
      a. The float property: "take[s] an element in normal flow and place[s] it as far to the left or right of the containing element as possible."
      b. "When you use the float property, you should also use the width property to indicate how wide the floated element should be."
      c. Often used to place boxes elements in line with each other.
      d. Watch the height of each element, because it can block other elements from floating as you'd like. 
      e. The clear property: "The clear property allows you to say that no element (within the same containing element) should touch the left or right- hand sides of a box." It takes values of left, right, both, or none.
      f. Problem with parents: if all its child elements are floated, it will be treated as if it had no content, making it flat. To fix, do the following:
        i. "The overflow property is given a value auto."
        ii. "The width property is set to 100%."
      g. Creating multi-column layouts
        i. Use a div or other block-level element
        ii. set the width, float, and margin properties. 
        iii. example:
          .column1of3, .column2of3, .column3of3 {
              width: 300px;
              float: left;
              margin: 10px;}
    6. The z-index property:
      a. "Allows you to control which box appears on top."
      b. "When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page."
      c. "Its value is a number, and the higher the number the closer that element is to the front."
      d. "If you are familiar with desktop publishing packages, it is the equivalent of using the 'bring to front' and 'send to back' features."

II. Screen Sizes: because they differ widely, you have to keep this in mind.

  A. Resolution = dots per inch. The higher the resolution, the smaller the text, so most mobile devices have screens with higher resolutions.
  B. Page sizes
    1. Width: Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide.
    2. Height: much harder to judge.
      a. "The area of the page that users would see without scrolling was often referred as being “above the fold” (a term newspapers had originally coined to describe the area of the front page you would see if the paper were folded in half)."
      b. "It is now recognized that if someone is interested in the content of the page, they are likely to scroll down to see more. Having said which [sic], usability studies have shown that visitors can judge a page in under a second so it is still important to let new visitors know that the site is relevant to them and their interests."
      c. "As a result, many designs still try to let the user know what the site is about within the top 570- 600 pixels, as well as hint at more content below this point. But do not try to cram too much into that top area."
    C. Fixed-width layouts
      1. "[D]o not change size as the user increases or decreases the size of their browser window."
      2. Advantages:
        a. "Pixel values are accurate at controlling size and positioning of elements."
        b. "The designer has far greater control over the appearance and position of items on the page than with liquid layouts."
        c. "You can control the lengths of lines of text regardless of the size of the user's window."
        d. "The size of an image will always remain the same relative to the rest of the page."
      3. Disadvantages:
        a. "You can end up with big gaps around the edge of a page."
        b. "If the user's screen is a much higher resolution than the designer's screen, the page can look smaller and text can be harder to read."
        c. "If a user increases font sizes, text might not fit into the allotted spaces."
        d. "The page will often take up more vertical space than a liquid layout with the same content."
      4. "To create a fixed-width layout the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too)."
    D. Liquid layouts: "stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages."
      1. Advantages
        a. "Pages expand to fill the entire browser window so there are no spaces around the page on a large screen."
        b. "If the user has a small window, the page can contract to fit it without the user having to scroll to the side."
        c. "The design is tolerant of users setting font sizes larger than the designer intended (because the page can stretch)."
      2. Disadvantages
        a. "If you do not control the width of sections of the page then the design can look very different than you intended, with unexpected gaps around certain elements or items squashed together."
        b. "If the user has a wide window, lines of text can become very long, which makes them harder to read."
        c. "If the user has a very narrow window, words may be squashed and you can end up with few words on each line."
        d. "If a fixed width item (such as an image) is in a box that is too small to hold it (because the user has made the window smaller) the image can overflow over the text."
      3. "The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen."

III. Learn the difference between fixed width and liquid layouts, and how they are created.

IV. Find out how designers use grids to make their page designs look more professional.

[<--back](201week1.md)

[<--home-->](../../README.md)
