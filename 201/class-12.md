# charts.js

[Return to 201 TOC](201TOC.md)

*Resource: <https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/>

## Easily create stunning animated charts with chart.js

- Chart.js is a JavaScript plugin that uses the HTML5 canvas element to draw graphs onto the page.
- The `chart.min.js` needs to be imported in the head section of the HTML file with `<script src=”chart.min.js”></script>`
- Add a canvas element to the HTML in the body section giving it an ID, width and height. Example: `<canvas id=”buyers” width=”600” height=”400”></canvas>`
- In the script, a variable grabbing the window into the DOM is created using the ID from the canvas element in the HTML and then `.getContext()` to get the drawing context usually is ‘2d’ for a 2 dimensional rendering context. Example `let buyers = document.getElementById(‘buyers’).getContext(‘2d’);`
- Next you create a new char object providing it the variable created above then chaining the type of graph and providing this the data object for the graph. The data object will include the labels, styling & data set. Example: `new Chart(buyers).Line(buyerData);`
- Above the 2 lines, a new object is created that has the name of the data set. The name of this object is the value you pass into the `.Line` method. Example:

``` javascript
let buyerData = {
  labels : [“January”, “February”, “March”, “April”, “May”, “June”],
  datasets : [
    {
        fillColor: “rgba(172,194,132,0.4)”,
        strokeColor : “#ACC26D”,
        pointColor : “#fff”,
        pointStrokeColor : “#9DB86D”,
        data: [203, 156, 99, 251, 305, 247]
    }
  ]
}
```

- You can change the graph type to a pie chart by changing the `.Line` to a `.Pie` passing in the data and a second parameter of options.
- The pie data is an array containing objects with the value and other key/value pairs like color.
- The options is also an object containing key/value pairs to define the options needed to configure the pie chart.
- For a bar graph you specify `.Bar` and pass in the dataset variable.
- This dataset variable now has additional data sets in it to specify each bar.


[Return to 201 TOC](201TOC.md)

[Return to Main Page](../README.md)
