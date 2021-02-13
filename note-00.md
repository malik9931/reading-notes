## Responsive Web Design
![aksm](https://kbworks.org/wp-content/uploads/2019/05/responsive-web-design-kb-works.jpg)

#### Responsive Web design is the approach that suggests that design and development should respond to the user's behavior and environment based on screen size, platform and orientation. ... In other words, the website should have the technology to automatically respond to the user's preferences



### Flexible Layouts
![kalsj](https://www.metropublisher.com/downloads/160/download/varied-layouts.png?cb=92d9cbb9db3f30456b73a5705eb8b243&w=640)

##### A flexible, or "liquid," approach to page layout attempts to accommodate the diversity of display environments. Rather than serving only the "most common" display dimensions and the "typical" user, a flexible layout adapts to different viewing conditions and different user requirements.


### Media Queries
![Media Queries](https://www.seobility.net/en/wiki/images/6/6f/Media-Queries.png)

Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.


Here's an example of a media query that returns the content when the device's width is less than or equal to 100px:

@media (max-width: 100px) { /* CSS Rules */ }

and the following media query returns the content when the device's height is more than or equal to 350px:

@media (min-height: 350px) { /* CSS Rules */ }

Remember, the CSS inside the media query is applied only if the media type matches that of the device being used.



### Make Typography Responsive
![xvvs](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSPJPLYMuCLg03VksC9Ww4UaQ4-IV-FQQVOdQ&usqp=CAU)

Instead of using em or px to size text, you can use viewport units for responsive typography. Viewport units, like percentages, are relative units, but they are based off different items. Viewport units are relative to the viewport dimensions (width or height) of a device, and percentages are relative to the size of the parent container element.

The four different viewport units are:

vw (viewport width): 10vw would be 10% of the viewport's width.
vh (viewport height): 3vh would be 3% of the viewport's height.
vmin (viewport minimum): 70vmin would be 70% of the viewport's smaller dimension (height or width).
vmax (viewport maximum): 100vmax would be 100% of the viewport's bigger dimension (height or width).
Here is an example that sets a body tag to 30% of the viewport's width.

body { width: 30vw; }


## Floats
![dskm](https://i1.wp.com/css-tricks.com/wp-content/csstricks-uploads/web-layout.png?resize=540%2C240&ssl=1)

Floating elements are removed from the normal flow of a document and pushed to either the left or right of their containing parent element. It's commonly used with the width property to specify how much horizontal space the floated element requires.

#### Clearing the Float
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.

![lasj](https://i2.wp.com/css-tricks.com/wp-content/csstricks-uploads/clearedfooter.png?resize=540%2C230)
