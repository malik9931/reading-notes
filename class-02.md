# HTML book:
## Chapter 2: “Text” (pp.40-61)
When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.

### Markup Types:
1-	Structural markup: the elements that you can use to describe both headings and paragraphs.
2-	Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on.

### Structural Markup
Headings <h1> …….. <h6>
Paragraphs <p>….</p>
Bold & Italic <p>This is how we make a word appear <i>italic</i> and <b>bold</b>.</p>

Superscript (22) 2<sup>2</sup>

Subscript (22) 2<sub>2</sub>


White Space: <p>The moon is                        drifting away from Earth.</p>  

white space collapsing >>>>>>> The moon is drifting away from Earth


Line Breaks <br />
To add a line break inside the middle of a paragraph you can use the line break tag <br />.

Horizontal Rules <hr />
To create a break between themes


### Empty elements: elements that do not have any words between an opening and closing tag, An empty element usually has only one tag. Before the closing angled bracket of an empty element there will often be a space and a forward slash character.



### Semantic Markup

Strong (bold): <strong>Beware:</strong>

Emphasis (italic): <em>think</em>

Quotations: <blockquote> for long quote
   <q> for short quote

Abbreviations & Acronyms:
<abbr title="Professor">Prof</abbr>
<acronym title="National Aeronautics and Space Administration">NASA</acronym>

Changes to Content: <ins> inserted in the text, <del> deleted from text


## Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)
CSS Associates Style rules with HT ML elements.
A CSS rule contains two parts: a selector and a declaration.
Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties.


Using External CSS:
<link> HTML
The <link> element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.

<link href="css/styles.css" type="text/css" rel="stylesheet" />
Href					
This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).

type
This attribute specifies the type
of document being linked to. The
value should be text/css.

rel
This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet when
linking to a CSS file.



Using Internal CSS:
Use <style> in the head section.

CSS Selectors
 

The priorities of CSS Rules:
LAST RULE
SPECIFICITY
IMPORTANT (!important)


# JS book:
## Chapter 2: “Basic JavaScript Instructions” (pp.53-84):

It is best to keep JavaScript code in its own JavaScript
file. JavaScript files are text files (like HTML pages and
CSS style sheets), but they have the . j s extension.

The HTML <script> element is used in HTML pages
to tell the browser to load the JavaScript file

If you view the source code of the page in the browser,
the JavaScript will not have changed the HTML,
because the script works with the model of the web
page that the browser has created.

Statements are used in JavaScript to control its program flow.

Methods are actions that can be performed on objects. Object properties can be both primitive values, other objects, and functions.

EX: document.write(‘Good Evning’);

Every statement end by ;

The curly braces indicate the start and end of a code block. (Each code block could contain many more statements.)

JAVASCRIPT IS CASE SENSITIVE

/* for
Multi – line
Comments*/

// for one line comment


Defining Variable:
var nameOfVariable;
nameOfVariable = something (string , number, boolean);

ARRAYS:
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

Array literal
var colors;
colors = ['white', 12 , True];




### Array constructor
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



The script is a series of instructions that follow by a computer to achieve a goal.

EXPRESSIONS:
An expression evaluates into (results in) a single value.

OPERATORS:
Operators allow programmers to create a single value from one or more values. 

Operators type:

1-	ASSIGNMENT OPERATORS
2-	ARITHMETIC OPERATORS
3-	STRING OPERATORS: +
4-	COMPARISON OPERATORS: > < ==
5-	LOGICAL OPERATORS

## Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162):
Comparison Operators
Comparison operators are used in logical statements to determine equality or difference between variables or values.

==	equal to
===	equal value and equal type
!=	not equal
!==	not equal value or not equal type
>	greater than
<	less than
>=	greater than or equal to
<=	less than or equal to




Logical Operators
Logical operators are used to determine the logic between variables or values.

&&	and
||	or
!	not


