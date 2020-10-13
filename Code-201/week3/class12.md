# Code 201 | Chart.JS and the Canvas API

## Class 12 Reading Notes

### [Chart.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/){:target="_blank" rel="noopener"}

I. Getting started

  A. Chart.js = a JavaScript plugin that uses the built-in canvas element in HTML5 to draw the graph onto the page.

  B. Getting started

    1. Download chart.js.
    2. Copy the Chart.min.js out of the unzipped folder and into your directory.
    3. Import the script into your index like this: `<script src='Chart.min.js'></script>`

II. Drawing charts

  A. Drawing a line chart

    1. Create a canvas element in our HTML: ` <canvas id="buyers" width="600" height="400"></canvas> `
    2. Write a script that will retrieve the context of the canvas: 
      ```
          <script>
            var buyers = document.getElementById('buyers').getContext('2d');
            new Chart(buyers).Line(buyerData);
          </script>
      ```
    3. Inside the same script tags we need to create our data (immediately above the line that begins ‘var buyers=’):
      ```
          var buyerData = {
        labels : ["January","February","March","April","May","June"],
        datasets : [
          {
            fillColor : "rgba(172,194,132,0.4)",
            strokeColor : "#ACC26D",
            pointColor : "#fff",
            pointStrokeColor : "#9DB86D",
            data : [203,156,99,251,305,247]
          }
        ]
      }
      ```
  B. Drawing a pie chart

    1. First, create the canvas element

      ` <canvas id="countries" width="600" height="400"></canvas> `

    2. Get the context and instantiate the chart

      ` var countries= document.getElementById("countries").getContext("2d");
        new Chart(countries).Pie(pieData, pieOptions); `

    3. Create the data

      ```
            var pieData = [
        {
          value: 20,
          color:"#878BB6"
        },
        {
          value : 40,
          color : "#4ACAB4"
        },
        {
          value : 10,
          color : "#FF8153"
        },
        {
          value : 30,
          color : "#FFEA88"
        }
      ];
      ```
    4. Add options after the pie data

    ```
          var pieOptions = {
        segmentShowStroke : false,
        animateScale : true
      }
    ```
  C. Drawing a bar chart

    1. Add the canvas element
    ` <canvas id="income" width="600" height="400"></canvas> `

    2. Retrieve the element and create the graph
    ```
    var income = document.getElementById("income").getContext("2d");
    new Chart(income).Bar(barData);
    ```
    3. Add the data
    ```
        var barData = {
      labels : ["January","February","March","April","May","June"],
      datasets : [
        {
          fillColor : "#48A497",
          strokeColor : "#48A4D1",
          data : [456,479,324,569,702,600]
        },
        {
          fillColor : "rgba(73,188,170,0.4)",
          strokeColor : "rgba(72,174,209,0.4)",
          data : [364,504,605,400,345,320]
        }

      ]
    }
    ```
III. Drawbacks

  A. No labels built in; you have to create and position them yourself. 
  B. [Empty]

### The Canvas API

I. [Basic Usage of Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage){:target="_blank" rel="noopener"}

  A. The `<canvas>` element

    1. Basic format: `<canvas id="tutorial" width="150" height="150"></canvas>`
    2. Only two attributes: 
    
      a. Width and height, which are optional and can be set by manipulating the DOM.
      b. Default: 300px x 150x
      c. "If the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted."

    3. Styling

      a. "The <canvas> element can be styled just like any normal image (margin, border, background…).
      b. "These rules, however, don't affect the actual drawing on the canvas."
      c. "When no styling rules are applied to the canvas it will initially be fully transparent."

  B. Fallback content

    1. Displayed in older browswers that can't read canvas.
    2. "Just insert the alternate content inside the <canvas> element. Browsers that don't support <canvas> will ignore the container and render the fallback content inside it. Browsers that do support <canvas> will ignore the content inside the container, and just render the canvas normally."
    3. Example: 
      ```
      <canvas id="clock" width="150" height="150">
        <img src="images/clock.png" width="150" height="150" alt=""/>
      </canvas>
      ```
    4. A closing tag is required.

  C. The rendering contexts

    1. getContext()
    
      a. Takes one parameter: the type of context, e.g., '2d'
      b. A node on the html doc is used to attach to the DOM.
      c. Example:
      ```
      var canvas = document.getElementById('tutorial');
      var ctx = canvas.getContext('2d');

II. [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes){:target="_blank" rel="noopener"}

  A. 

III. [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors){:target="_blank" rel="noopener"}

IV. [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text){:target="_blank" rel="noopener"}

[<--back](201week3.md)

[<--home-->](../../README.md)
