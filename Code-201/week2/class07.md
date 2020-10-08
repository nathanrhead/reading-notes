# Code 201 | Object-oriented Programming & HTML Tables

## Class 07 Reading Notes

## Domain Modeling (from the CF archives)

I. Definition:
  
  A. "The process of creating a conceptual model in code for a specific problem."
  B. "A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain."
  C. "An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model."
  D. "A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams."

II. Defining a constructor and initializing properties

  A. "To define the same properties [among] many objects, you'll want to use a constructor function."
  B. Example:
  
  `var EpicFailVideo = function(epicRating, hasAnimals) {`
  `this.epicRating = epicRating;`
  `this.hasAnimals = hasAnimals;`
    `}`
    `var parkourFail = new EpicFailVideo(7, false);`
    `var corgiFail = new EpicFailVideo(4, true);`
    `console.log(parkourFail);`
    `console.log(corgiFail);`

  C. "When the function is called, the data inside these parameters are stored inside the this.epicRating and this.hasAnimals properties respectively. Storing data within properties ensures any newly created object can access that data later."
  D. "After the constructor function definition, two objects are instantiated with the new keyword and their properties are initialized by calling the EpicFailVideo constructor function. After being instantiated and initialized, these objects are stored inside the parkourFail and corgiFail variables."
  E. Summary of the steps involved in object-oriented programming:
    
    1. "The new keyword instantiates (i.e. creates) an object."
    2. "The constructor function initializes properties inside that object using the this variable."
    3. "The object is stored in a variable for later use."

III. To model random human behavior, use Math.random as so:
`
    `var EpicFailVideo = function(epicRating, hasAnimals) {`
      `this.epicRating = epicRating;`
      `this.hasAnimals = hasAnimals;`
    `}`
`
    `EpicFailVideo.prototype.generateRandom = function(min, max) {`
      `return Math.floor(Math.random() * (max - min + 1)) + min;`
    `}`
`
    `var parkourFail = new EpicFailVideo(7, false);`
   ` var corgiFail = new EpicFailVideo(4, true);`
`
    `console.log(parkourFail.generateRandom(1, 5));`
    `console.log(corgiFail.generateRandom(1, 5));`
    `

## Chapter 6: Tables (pp. 126 - 145) from _HTML & CSS_ by Jon Duckett

I. Use the four key elements for creating tables

  A. `<table>`: "The `<table>` element is used to create a table. The contents of the table."
  B. `<tr>`:

    1. "You indicate the start of each row using the opening <tr> tag. (The tr stands for table row.)"
    2. "It is followed by one or more <td> elements (one for each cell in that row)."
    3. These are not self-closing tags.

  C. `<td>`: "Each cell of a table is represented using a `<td>` element. (The td stands for table data.)"
  
  D. `<th>`: table heading

    1. "The <th> element is used just like the <td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)"
    2. "Even if a cell has no content, you should still use a <td> or <th> element to represent the presence of an empty cell otherwise the table will not render correctly."
    3. "Using <th> elements for headings helps people who use screen readers, improves the ability for search engines to index your pages, and also enables you to control the appearance of tables better when you start to use CSS."
    4. "You can use the scope attribute on the <th> element to indicate whether it is a heading for a column or a row. It can take the values: row to indicate a heading for a row or col to indicate a heading for a column."

II. Other elements

  A. Spanning columns: "Sometimes you may need the entries in a table to stretch across more than one column. The colspan attribute can be used on a `<th>` or `<td>` element and indicates how many columns that cell should run across."
  B. Spanning rows: "ou may also need entries in a table to stretch down across more than one row. The rowspan attribute can be used on a `<th>` or `<td>` element to indicate how many rows a cell should span down the table."
  C. Long tables

    1. <thead>: "The headings of the table should sit inside the <thead> element." So, <table><thead><tr><th><</th></tr></thead>
    2. <tbody>: "The body should sit inside the <tbody> element."
    3. <tfoot>: "The footer belongs inside the <tfoot> element."

## Chapter 3: Functions, Methods, and Objects (pp. 106 - 144) from _JavaScript & jQuery_ by Jon Duckett

I. Creating an object: constructor notation

  A. 


  [<--back](201week2.md)

[<--home-->](../../README.md)
