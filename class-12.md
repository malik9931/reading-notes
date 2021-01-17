## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS

The great things about Chart.js are that it’s simple to use and really very flexible.

![ajs](https://cdn.mos.cms.futurecdn.net/S5bicwPe8vbP9nt3iwAwwi.jpg)


## Basic usage of canvas

''' <canvas id="tutorial" width="150" height="150"></canvas> '''


## The grid:

![dsd](https://mdn.mozillademos.org/files/224/Canvas_default_grid.png)

<canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines)

 All other shapes must be created by combining one or more paths.

### to draw a rectangles using canvas:

 fillRect(x, y, width, height)
Draws a filled rectangle.

strokeRect(x, y, width, height)
Draws a rectangular outline.

clearRect(x, y, width, height)
Clears the specified rectangular area, making it fully transparent.


### Here are the functions used to perform drawing a path:

beginPath()
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.
closePath()
Adds a straight line to the path, going to the start of the current sub-path.
stroke()
Draws the shape by stroking its outline.
fill()
Draws a solid shape by filling the path's content area.



## Making combinations
There's no limitation to the number or types of paths you can use to create a shape.

![ds](https://mdn.mozillademos.org/files/9849/combinations.png)





## Applying styles and colors

fillStyle = color
Sets the style used when filling shapes.

strokeStyle = color
Sets the style for shapes' outlines.

![cxz](https://mdn.mozillademos.org/files/5417/Canvas_fillstyle.png)

![fd](https://mdn.mozillademos.org/files/253/Canvas_strokestyle.png)

