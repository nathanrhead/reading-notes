# Code 301 | CSS Grin

## Class 04 Reading Notes

### ["Grid Garden"](https://cssgridgarden.com/)

I. By Codepig (like the froggy flexbox game).

II. A game in 28 steps to familiarize you with using CSS grid.

III. Understanding and Using CSS Grid?

  A. You lay out an x-y (or row-column) grid by indicating the following on a container with a property of display and a value of grid:

    1. grid-template-columns: 20% 20% 20% 20% 20% = 5 columns each of 20% of the width of the parent container.

    2. grid-template-rows: 20% 20% 20% 20% 20% = 5 columns each of 20% of the width of the parent container.

  B. grid-column-start: 3 = will position your element at the top of the third column.

  C. grid-column-end: 4 = will stretch your element from 1 to 4 (through the third column).

  D. grid-column-end: 2 = when your object is already at grid-column-start: 5, will spread it across the second, third, and fourth columns.

  E. You can use negative values on grid-column-end, too, and they'll spread elements from the left to the right.

  F. You can use negative values with grid-column-start, and they will move your element that number of spaces to the right, e.g., -3 moves the element three spaces from the first column, or to the head of column four.

  G. Span: this value with a number after it, e.g., span 2, will extend your element over two columns (when used with grid-column-end/start).

  H. grid-column: 2 / 4 = is shorthand for grid-column-start and grid-column-end; this example will start the grid item on the second column and end it on the fourth; span also works with this shorthand.

  I. grid-row-start works like column-start only on the y axis.

  J. grid-row is the shorthand for grid-row-start/end; shorthand may be used with only one value.

  K. grid-area
  
    i. a shorthand for using grid-column/row to cover an two-dimensional area;

    ii. excepcts 4 values separated by back slashes indicating row-start / column-start / row-end / column-end.

  L. Grid items can overlap eachother.

  M. Overriding the order of items using the order property:  

    i. default order for all items is 0;

    ii. set it to any positive or negative value (as with z-index);

  N. grid-template-columns (and rows) can be set with a shortcut for repeating column widths, e.g., grid-template-columns: repeat(5, 20%); you can also use pixels and ems or mix units together.

  O. New unit of measurement in grid = fr = the fractional

    i. "Each fr unit allocates one share of the available space."

    ii. "For example, if two elements are set to 1fr and 3fr respectively, the space is divided into 4 equal shares; the first element occupies 1/4 and the second element 3/4 of any leftover space."

    iii. "When columns are set with pixels, percentages, or ems, any other columns set with fr will divvy up the space that's left over."

  [<--back](301week1.md)

[<--home-->](../../README.md)
