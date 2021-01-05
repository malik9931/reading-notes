HTML book:
Chapter 3: “Lists” (pp.62-73)
Three different types:
Ordered lists are lists where each item in the list is numbered. <ol> >>><li>

Unordered lists are lists that begin with a bullet point. <ul> >>><li>


Definition lists are made up of a set of terms along with the definitions for each of those terms.
<dl> / Inside the <dl> element you will usually see pairs of <dt> (the definition
term) and <dd> (contain the definition)elements.


Nested Lists:
You can put a second list inside an <li> element to create a sublist or nested list.

Chapter 13: “Boxes” (pp.300-329)

Box Dimensions
The most popular ways to specify the size of a box are:
1-	Pixels: most popular use by designers.
2-	Percentages: the size of the box is relative to the size of the browser window.
3-	Ems: the size of the box is based on the size of text within it.

Limiting Width
min-width, max-width

Limiting Height
min-height, max-height

Overflowing Content: 
Overflow: The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
Hidden , Scroll 

Border, Margin & Padding

Border: Every box has a border.

Margin: Margins sit outside the edge of the border.

Padding: is the space between the border of a box and any content contained within it.






Border width: px, thin, medium, thick.

border-style: solid / dashed / dotted / double / groove / ridge / inset / hidden / none

Centering Content:
text-align: center;

Display property: 
 

And (none).


Visibility Property: hidden or visible
visibility: hidden;

CSS3 has introduced the ability to create image borders and rounded borders.

Elliptical Shapes:
border-radius:

border-top-left-radius: 80px 50px;


JS book:

ARRAYS:
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

Array literal
var colors;
colors = ['white', 12 , True];




Array constructor
var colors = new Array('white ' ,
'black',
'custom ' );

Each item in an array is automatically given a number called an index.


ACCESSING ITEMS IN AN ARRAY
var itemThree;
itemThree = colors [ 2] ;

NUMBER OF ITEMS IN AN ARRAY
var numColors ;
numColors =colors. length;


