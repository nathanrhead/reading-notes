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
        1. Display: "llows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page."
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

III. Set margins and padding for boxes

IV. Show and hide boxes


---

## _JavaScript & jQuery_ by Jon Duckett

### Review from Reading 02, Chapter 2: Basic JavaScript Instructions (pp. 70 - 73)

I. 

### Chapter 4: Decisions and Loops (starting from switch statements) (pp. 162 - 182)

I. 