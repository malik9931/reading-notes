# CSS GRID
CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. 

(Flexbox and Grid actually work very well together)

To get started you have to define a container element as a grid with display: grid, set the column and row sizes with grid-template-columns and grid-template-rows, and then place its child elements into the grid with grid-column and grid-row. 

#### Important Terminology
###### Grid Container : class="container"

```<div class="container">
  <div class="item item-1"> </div>
  <div class="item item-2"> </div>
  <div class="item item-3"> </div>
</div>
```

###### Grid Item : class="item"

```<div class="container">
  <div class="item item-1"> </div>
  <div class="item item-2"> </div>
  <div class="item item-3"> </div>
</div>
```

###### Grid Item : class="item"

```<div class="container">
  <div class="item"> </div>
  <div class="item">
    <p class="sub-item"> </p>
  </div>
  <div class="item"> </div>
</div>
```

###### Grid Line
![fs](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-line.svg)

###### Grid Cell
![ad](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-cell.svg)

###### Grid Track
![dsf](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-track.svg)

###### Grid Area
![dsf](https://css-tricks.com/wp-content/uploads/2018/11/terms-grid-area.svg)



#### Regular expressions
Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern (i.e. a specific sequence of ASCII or unicode characters).

One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).

cheatsheet for Regular expressions:
https://regexr.com/

