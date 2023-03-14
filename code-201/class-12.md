# Title of Article

## JavaScript Canvas
[Source](https://www.javascripttutorial.net/web-apis/javascript-canvas/)

Notes
`<canvas>` was first introduced in HTML5. It requires at least two attributes: `width` (x-axis) and `height` (y-axis). width and height determine the number of pixels available in each direction (x or y axis). Other attributes: `id`. disallows CSS styles?

`canvas.width` and `canvas.height` are ways to access canvas element via its DOM properties. 

declared using `const`

Any content between opening and closing content will only display if the browser does not support

Canvas .methods:
1. `.getContext()` - returns a render context object (also access the drawing context). takes one argument which is type of context e.g., 2D 
2. `.fillStyle` - fill in with color like Paint
3. `.strokeStyle` - fill in color of border?
4. `.fillRect()` - (y1, y2, x1, x2)? 1 is starting value, 2 is ending value
5. `.strokeRect()` - (y1, y2, x1, x2)?

[Canvas quadrant example](https://www.javascripttutorial.net/wp-content/uploads/2020/09/JavaScript-Canvas.png)

DOM .methods (refresher):
1. `.querySelector()` - example was declared with `const`

Q&A
1. What does the `<canvas>` allow a developer to achieve? Allows the developer to draw shapes, text, images, and other objects

2. What is the importance of the closing `</canvas>` tag? To insert Fallback Content in case the browser does not support the `<canvas>` element

3. Explain what the `getContext()` method does. Renders the drawing onto the canvas


## Chart.js Documentation
[Source](https://www.chartjs.org/docs/latest/)

Notes

Chart.js is a charting library and currently the most popular. Animations are turned on by default. Allows the developer to tell a story with data. 

suited for large datasets, might be great for data scientists. 

used in conjunction with Chart.js 

Data decimation - not sure what this means.....

Built-in chart types: area, bar, bubble, doughnut/pie, line, mixed-chart, polar area, radar, scatter

Community built chart types:

Q&A
1. What is Chart.js and how it can be brought into your project? It appears to be a data visualization tool used for large datasets to tell a story in conjunction with `<canvas>`

2. List 3 different Chart types you can create using Chart.js. Bubble, Doughnut, Mixed-chart

## Easily Create Stunning Animated Charts with Chart.js
[Source](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

Notes

Chart Example (`.Line()`)

needs labels: , datasets: , fillColor: , strokeColor: , pointColor: , pointStrokeColor: , data:

`<script>`
 
 `var buyers = document.getElementById('buyers').getContext('2d');`
 
 `new Chart(buyers).Line(buyerData);`

`</script>`

`new Chart(buyers).Line(buyerData);`

Pie Example (`.Pie(data, options)`)

`new Chart(countries).Pie(pieData, pieOptions);`

has value: color pairs



Q&A

1. What are some advantages to displaying data via a chart over a table? simple to use, really flexible, and they're more visually appealing

2. How could Chart.js aid your previously created applications visually? It would allow me to tell a story with large datasets

## Bookmark and Review

[Drawing Shapes With Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

[Applying Styles and Colors - Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

[Drawing Text - Canvas API](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

### Things I want to know

- is Chart.js comparable to pandas in python?