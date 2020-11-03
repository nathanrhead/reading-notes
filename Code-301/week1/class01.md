# Code 301 | Responsive Web Design and Floats

## Class 01 Reading Notes

### Shay Howe's Intro to RWD

I. Responsive Web Design defined

  A. Introduction
  
    1. Definition: RWD is "the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop."
  
    2. Ethan Marcotte coined the term in a book worth reading, called _Responsive Web Design_."

  B. Responsive v. Adaptive v. Mobile

    1. Responsive: a website that is built to respond to changing factors; best used in combination with adaptive.

    2. Adaptive: a website that is built with particular factors in mind; best used in combination with responsive.

    3. Mobile: a site on its own domain built specifically for mobile devices; not recommended on its own.

  C. Three main components of RWD

    1. Flexible Layouts: building with a flexible grid that can dynamically be resized as needed and relative units, such as percentages and ems. 

      a. CSS3 introduced new relative units, including the following:

        i. vw = viewport width

        ii. vh = viewport height

        iii. vmin = minimum of the viewport's height and width

        iv. vmax = maximum of the viewport's height and width

      b. Determining the proportions of a flexible layout using relative values: "tak[e] the target width of an element and divid[e]] it by the width of it’s parent element. The result is the relative width of the target element."

II. Media Queries: "Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation."

  A. Three types

    1. @media: used in an existing style sheet. [The preferred method, used to avoid additional http requests.]

    2. @import: used to import a new style sheet.

    3. Link in HTML to a new style sheet. 

  B. Type plus expression

  C. Common media types

    1. all, screen, print, tv, braille.

    2. Default = screen.

    3. "When a media feature and value allocate to true, the styles are applied. If the media feature and value allocate to false the styles are ignored."

  D. Logical operators in media queries

    1. and, not, only (as well as an unspoken "or" when you use commas between options)

    2. Example: @media all and (min-width: 800px) and (max-width: 1024px) {...}

  E. Media features: "identify what attributes or properties will be targeted within the media query expression."

    1. height and width media features: used to find the h and w of a viewport and to set the min and max, using any length, relative or absolute.

    2. orientation: landscape or portrait.

    3. aspect-ratio: "The aspect-ratio and device-aspect-ratio features specifies the width/height pixel ratio of the targeted rendering area or output device. The value for the aspect ratio feature consist of two positive integers separated by a forward slash. The first integer identifies the width in pixels while the second integer identifies the height in pixels."

    4. pixel-ratio: used to identify high-res displays. 

    5. resolution: "specifies the resolution of the output device in pixel density, also known as dots per inch or DPI."

III. Mobile First

  A. "[U]sing styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows."

  B. "The operating belief behind mobile first design is that a user on a mobile device, commonly using a smaller viewport, shouldn’t have to load the styles for a desktop computer only to have them over written with mobile styles later. Doing so is a waste of bandwidth."

  C. "Additionally, downloading unnecessary media assets can be stopped by using media queries. Generally speaking, avoiding CSS3 shadows, gradients, transforms, and animations within mobile styles isn’t a bad idea either. When used excessively, they cause heavy loading and can even reduce a device’s battery life."



### All About Floats



### Don't-Overthink-It Grids


### CSS Floats Explained by Riding an Escalator


### SMACCS Official Documentation

[<--back](301week1.md)

[<--home-->](../../README.md)
