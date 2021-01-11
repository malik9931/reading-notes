### Domain Modeling
Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.



#### Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function.


This is object-oriented programming in JavaScript at its most fundamental level.

1. The new keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the this variable.
3. The object is stored in a variable for later use.


### “Tables” (pp.126-145):
A table represents information in a grid format. Examples of tables include financial reports, TVschedules, and sports results.

Each block in the grid is referred
to as a table cell. In HTML a
table is written out row by row.

~~~

<table>                                           
The <table> element is used                   
to create a table. The contents                           
of the table are written out row            
by row.     

<tr>
You indicate the start of each
row using the opening <tr> tag.
(The tr stands for table row.)
It is followed by one or more
<td> elements (one for each cell
in that row).
At the end of the row you use a
closing </tr> tag.

<td>
Each cell of a table is
represented using a <td>
element. (The td stands for
table data.)
At the end of each cell you use a
closing </td> tag.

<th>
The <th> element is used just
like the <td> element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)


Notice:
Even if a cell has no content,
you should still use a <td> or
<th> element to represent
the presence of an empty cell
otherwise the table will not
render correctly.


##### Spanning ColumnS
Sometimes you may need the entries in a table to stretch across more than one column.

USE: 
~~~
<td colspan="2">Geography</td>
~~~

##### Spanning Rows
You may also need entries in the table to stretch down across more than one row. The rowspan attribute can be used on a <th> or <td> element to indicate how many rows a cell should span down the table.

~~~
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
~~~

##### Long Tables
<thead>
The headings of the table should
sit inside the <thead> element.
<tbody>
The body should sit inside the
<tbody> element.
<tfoot>
The footer belongs inside the
<tfoot> element.

~~~
~~~
### “Functions, Methods, and Objects” (pp.106-144)
CREATING MANY OBJECTS:
CONSTRUCTOR NOTATION

Sometimes you will want several objects to represent similar things.
Object constructors can use a function as a template for creating objects.
First, create the template with the object's properties and methods.


(The+= operator is used to add content to an existing variable.)

##### ADDING AND REMOVING PROPERTIES
Once you have created an object
(using literal or constructor
notation), you can add new
properties to it.

~~~
var hotel = {
name : 'Park' ,
rooms : 120,
booked : 77.
} ;
hotel .gym = t rue;
hotel .pool = fal se;
delete hotel .booked;
~~~

THIS (IT IS A KEYWORD)
The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates.
