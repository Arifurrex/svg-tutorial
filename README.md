Welcome to the svg-tutorial wiki!
![Screenshot 2022-11-27 192634](https://user-images.githubusercontent.com/48369328/204150527-7298ce36-7749-4e4b-8fad-088aeecbcad3.png)

# SVG
Scalable Vector Graphics

SVG defines vector-based graphics in XML format.

```html
<svg xmlns="http://www.w3.org/2000/svg">
    <ellipse cx="10" cy="10" rx="10" ry="10" style=""/>
   </svg>
```

## What is SVG?
* SVG stands for Scalable Vector Graphics
* SVG is used to define vector-based graphics for the Web
* SVG defines the graphics in XML format
* Every element and every attribute in SVG files can be animated
* SVG is a W3C recommendation
* SVG integrates with other W3C standards such as the DOM and XSL

### Creating SVG Images
SVG images can be created with any text editor, but it is often more convenient to create SVG images with a drawing program, like [Inkscape](http://inkscape.org/).







# SVG in HTML
You can embed SVG elements directly into your HTML pages.

Embed SVG Directly Into HTML Pages

```html
<svg width="100" height="100">
     <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```


## SVG Code explanation:
* An SVG image begins with an <svg> element
* The width and height attributes of the <svg> element define the width and height of the SVG image
* The <circle> element is used to draw a circle
* The cx and cy attributes define the x and y coordinates of the center of the circle. If cx and cy are not set, the circle's center is set to (0, 0)
* The r attribute defines the radius of the circle
* The stroke and stroke-width attributes control how the outline of a shape appears. We set the outline of the circle to a 4px green "border"
* The fill attribute refers to the color inside the circle. We set the fill color to yellow
* The closing </svg> tag closes the SVG image
* Note: Since SVG is written in XML, all elements must be properly closed!


# SVG Rectangle<rect>
## SVG Shapes
### SVG has some predefined shape elements that can be used by developers:
* Rectangle <rect>
* Circle <circle>
* Ellipse <ellipse>
* Line <line>
* Polyline <polyline>
* Polygon <polygon>
* Path <path>

The following chapters will explain each element, starting with the rect element.

```html
SVG Rectangle - <rect>
<svg width="400" height="100">
    <rect width="300" height="100" style="fill:aqua;stroke-width:3;stroke:red"/>
</svg>
```


## Code explanation:
* The width and height attributes of the <rect> element define the height and the width of the rectangle
* The style attribute is used to define CSS properties for the rectangle
* The CSS fill property defines the fill color of the rectangle
* The CSS stroke-width property defines the width of the border of the rectangle
* The CSS stroke property defines the color of the border of the rectangle

Another example :

```html

<svg width="400" height="180">
    <rect x="50" y="20" width="150" height="150"
     style="fill:aqua;stroke-width:3;stroke:red;fill-opacity:0.1;stroke-opacity:0.9"/>

  </svg>

````

### Code explanation:
* The x attribute defines the left position of the rectangle (e.g. x="50" places the rectangle 50 px from the left margin)
* The y attribute defines the top position of the rectangle (e.g. y="20" places the rectangle 20 px from the top margin)
* The CSS fill-opacity property defines the opacity of the fill color (legal range: 0 to 1)
* The CSS stroke-opacity property defines the opacity of the stroke color (legal range: 0 to 1)

### Another example:

```html
 <svg width="400" height="180">
    <rect x="50" y="20" width="150" height="150"
    style="fill:blue;stroke:pink;stroke-width:5;opacity:0.5" />
  </svg>

```

## Code explanation:

The CSS opacity property defines the opacity value for the whole element (legal range: 0 to 1)



### Another example:

```html
  <svg width="400" height="180">
    <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
    style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
 </svg>

````

### Code explanation:
The rx and the ry attributes rounds the corners of the rectangle











# SVG <circle>
## SVG Circle - <circle>

### The <circle> element is used to create a circle:
```html
 <svg height="100" width="100">
  <circle cx="50" cy="50" r="40" stroke="black" stroke-width="3" fill="red" />
</svg>
```

### Code explanation:
The cx and cy attributes define the x and y coordinates of the center of the circle. If cx and cy are omitted, the circle's center is set to (0,0)
The r attribute defines the radius of the circle



# SVG <ellipse>
An ellipse is closely related to a circle. The difference is that an ellipse has an x and a y radius that differs from each other, while a circle has equal x and y radius:


```html
 <svg height="140" width="500">
    <ellipse cx="200" cy="80" rx="100" ry="50"
    style="fill:yellow;stroke:purple;stroke-width:2" />
</svg
```



### Code explanation:
* The cx attribute defines the x coordinate of the center of the ellipse
* The cy attribute defines the y coordinate of the center of the ellipse
* The rx attribute defines the horizontal radius
* The ry attribute defines the vertical radius


### Example 2

The following example creates three ellipses on top of each other:

```html
<svg height="150" width="500">
  <ellipse cx="240" cy="100" rx="220" ry="30" style="fill:purple" />
  <ellipse cx="220" cy="70" rx="190" ry="20" style="fill:lime" />
  <ellipse cx="210" cy="45" rx="170" ry="15" style="fill:yellow" />
</svg>
```


### Example 3

The following example combines two ellipses (one yellow and one white):

```html
<svg height="100" width="500">
  <ellipse cx="240" cy="50" rx="220" ry="30" style="fill:yellow" />
  <ellipse cx="220" cy="50" rx="190" ry="20" style="fill:white" />
</svg>
```




# SVG <line>
## SVG Line - <line>
### The <line> element is used to create a line:

```html
<svg height="210" width="500">
  <line x1="0" y1="0" x2="200" y2="200" style="stroke:rgb(255,0,0);stroke-width:2" />
</svg>
```

### Code explanation:
* The x1 attribute defines the start of the line on the x-axis
* The y1 attribute defines the start of the line on the y-axis
* The x2 attribute defines the end of the line on the x-axis
* The y2 attribute defines the end of the line on the y-axis




# SVG <polygon>
## SVG Polygon - <polygon>
The <polygon> element is used to create a graphic that contains at least three sides.
Polygons are made of straight lines, and the shape is "closed" (all the lines connect up).
Polygon comes from Greek. "Poly" means "many" and "gon" means "angle".






```html
<svg height="210" width="500">
  <polygon points="200,10 250,190 160,210" style="fill:lime;stroke:purple;stroke-width:1" />
</svg>
```

### Code explanation:
The points attribute defines the x and y coordinates for each corner of the polygon

### Example 2
The following example creates a polygon with four sides:

```html
<svg height="250" width="500">
  <polygon points="220,10 300,210 170,250 123,234" style="fill:lime;stroke:purple;stroke-width:1" />
</svg>
```


### Example 3

Use the <polygon> element to create a star:
```html
<svg height="210" width="500">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:nonzero;" />
</svg>

```

### Example 4

Change the fill-rule property to "evenodd":

```html
<svg height="210" width="500">
  <polygon points="100,10 40,198 190,78 10,78 160,198"
  style="fill:lime;stroke:purple;stroke-width:5;fill-rule:evenodd;" />
</svg>

```

# SVG <polyline>
## SVG Polyline - <polyline>

### Example 1
The <polyline> element is used to create any shape that consists of only straight lines (that is connected at several points):

```html
<svg height="200" width="500">
  <polyline points="20,20 40,25 60,40 80,120 120,140 200,180"
  style="fill:none;stroke:black;stroke-width:3" />
</svg>
```

### Code explanation:
The points attribute defines the list of points (pairs of x and y coordinates) required to draw the polyline

### Example 2
Another example with only straight lines

```html
<svg height="180" width="500">
  <polyline points="0,40 40,40 40,80 80,80 80,120 120,120 120,160"
  style="fill:white;stroke:red;stroke-width:4" />
</svg>

```





# SVG <path>
## SVG Path - <path>
The <path> element is used to define a path.
The following commands are available for path data:
* M = moveto
* L = lineto
* H = horizontal lineto
* V = vertical lineto
* C = curveto
* S = smooth curveto
* Q = quadratic Bézier curve
* T = smooth quadratic Bézier curveto
* A = elliptical Arc
* Z = closepath
Note: All of the commands above can also be expressed with lower letters. Capital letters means absolutely positioned, lower cases means relatively positioned.

### Example 1

The example below defines a path that starts at position 150,0 with a line to position 75,200 then from there, a line to 225,200 and finally closing the path back to 150,0:

```html
<svg height="210" width="400">
  <path d="M150 0 L75 200 L225 200 Z" />
</svg>
```



### Example 2
Bézier curves are used to model smooth curves that can be scaled indefinitely. Generally, the user selects two endpoints and one or two control points. A Bézier curve with one control point is called a quadratic Bézier curve and the kind with two control points is called cubic.
The following example creates a quadratic Bézier curve, where A and C are the start and end points, B is the control point:

```html
<svg height="400" width="450">
  <path id="lineAB" d="M 100 350 l 150 -300" stroke="red"
  stroke-width="3" fill="none" />
  <path id="lineBC" d="M 250 50 l 150 300" stroke="red"
  stroke-width="3" fill="none" />
  <path d="M 175 200 l 150 0" stroke="green" stroke-width="3"
  fill="none" />
  <path d="M 100 350 q 150 -300 300 0" stroke="blue"
  stroke-width="5" fill="none" />
  <!-- Mark relevant points -->
  <g stroke="black" stroke-width="3" fill="black">
    <circle id="pointA" cx="100" cy="350" r="3" />
    <circle id="pointB" cx="250" cy="50" r="3" />
    <circle id="pointC" cx="400" cy="350" r="3" />
  </g>
  <!-- Label the points -->
  <g font-size="30" font-family="sans-serif" fill="black" stroke="none"
  text-anchor="middle">
    <text x="100" y="350" dx="-30">A</text>
    <text x="250" y="50" dy="-10">B</text>
    <text x="400" y="350" dx="30">C</text>
  </g>
</svg>
```

Complex? YES!!!! Because of the complexity involved in drawing paths it is highly recommended to use an SVG editor to create complex graphics.


### SVG <text>
## SVG Text - <text>
The <text> element is used to define a text.

### Example 1
Write a text:

Here is the SVG code:

```html
<svg height="30" width="200">
  <text x="0" y="15" fill="red">I love SVG!</text>
</svg>
```

### Example 2
Rotate the text:

Here is the SVG code:
```html
<svg height="60" width="200">
  <text x="0" y="15" fill="red" transform="rotate(30 20,40)">I love SVG</text>
</svg>

```



### Example 3
The <text> element can be arranged in any number of sub-groups with the <tspan> element. Each <tspan> element can contain different formatting and position.
Text on several lines (with the <tspan> element):

```html
<svg height="90" width="200">
  <text x="10" y="20" style="fill:red;">Several lines:
    <tspan x="10" y="45">First line.</tspan>
    <tspan x="10" y="70">Second line.</tspan>
  </text>
</svg>


Example 4
Text as a link (with the <a> element):

Here is the SVG code:
<svg height="30" width="200" xmlns:xlink="http://www.w3.org/1999/xlink">
  <a xlink:href="https://www.w3schools.com/graphics/" target="_blank">
    <text x="0" y="15" fill="red">I love SVG!</text>
  </a>
</svg>
```





### SVG Stroke Properties

SVG Stroke Properties
SVG offers a wide range of stroke properties. In this chapter we will look at the following:
* stroke
* stroke-width
* stroke-linecap
* stroke-dasharray
All the stroke properties can be applied to any kind of lines, text and outlines of elements like a circle.


SVG stroke Property
The stroke property defines the color of a line, text or outline of an element:

```html
<svg height="80" width="300">
  <g fill="none">
    <path stroke="red" d="M5 20 l215 0" />
    <path stroke="black" d="M5 40 l215 0" />
    <path stroke="blue" d="M5 60 l215 0" />
  </g>
</svg>
```

SVG stroke-width Property
The stroke-width property defines the thickness of a line, text or outline of an element:

```html
<svg height="80" width="300">
  <g fill="none" stroke="black">
    <path stroke-width="2" d="M5 20 l215 0" />
    <path stroke-width="4" d="M5 40 l215 0" />
    <path stroke-width="6" d="M5 60 l215 0" />
  </g>
</svg>
```

SVG stroke-linecap Property
The stroke-linecap property defines different types of endings to an open path:


```html
<svg height="80" width="300">
  <g fill="none" stroke="black" stroke-width="6">
    <path stroke-linecap="butt" d="M5 20 l215 0" />
    <path stroke-linecap="round" d="M5 40 l215 0" />
    <path stroke-linecap="square" d="M5 60 l215 0" />
  </g>
</svg>
```


SVG stroke-dasharray Property
The stroke-dasharray property is used to create dashed lines:


```html
<svg height="80" width="300">
  <g fill="none" stroke="black" stroke-width="4">
    <path stroke-dasharray="5,5" d="M5 20 l215 0" />
    <path stroke-dasharray="10,10" d="M5 40 l215 0" />
    <path stroke-dasharray="20,10,5,5,5,10" d="M5 60 l215 0" />
  </g>
</svg>

```


# SVG Filters
## SVG Filters
SVG Filters are used to add special effects to SVG graphics.
SVG Filter Elements
In the next chapters, we will only demonstrate a touch of the filter effects that are possible - and give you an idea of what can be done with SVG.
The available filter elements in SVG are:
* <feBlend> - filter for combining images
* <feColorMatrix> - filter for color transforms
* <feComponentTransfer>
* <feComposite>
* <feConvolveMatrix>
* <feDiffuseLighting>
* <feDisplacementMap>
* <feFlood>
* <feGaussianBlur>
* <feImage>
* <feMerge>
* <feMorphology>
* <feOffset> - filter for drop shadows
* <feSpecularLighting>
* <feTile>
* <feTurbulence>
* <feDistantLight> - filter for lighting
* <fePointLight> - filter for lighting
* <feSpotLight> - filter for lighting
Tip: You can use multiple filters on each SVG element!




# SVG Blur Effects
### <defs> and <filter>
All internet SVG filters are defined within a <defs> element. The <defs> element is short for definitions and contains definition of special elements (such as filters).
The <filter> element is used to define an SVG filter. The <filter> element has a required id attribute which identifies the filter. The graphic then points to the filter to use.
SVG <feGaussianBlur>

### Example 1
The <feGaussianBlur> element is used to create blur effects

```html
<svg height="110" width="110">
  <defs>
    <filter id="f1" x="0" y="0">
      <feGaussianBlur in="SourceGraphic" stdDeviation="15" />
    </filter>
  </defs>
  <rect width="90" height="90" stroke="green" stroke-width="3"
  fill="yellow" filter="url(#f1)" />
</svg>
```

### Code explanation:
* The id attribute of the <filter> element defines a unique name for the filter
* The blur effect is defined with the <feGaussianBlur> element
* The in="SourceGraphic" part defines that the effect is created for the entire element
* The stdDeviation attribute defines the amount of the blur
* The filter attribute of the <rect> element links the element to the "f1" filter

### SVG Drop Shadows
<defs> and <filter>
All SVG filters are defined within a <defs> element. The <defs> element is short for definitions and contains definition of special elements (such as filters).
The <filter> element is used to define an SVG filter. The <filter> element has a required id attribute which identifies the filter. The graphic then points to the filter to use.
SVG <feOffset>
### Example 1
The <feOffset> element is used to create drop shadow effects. The idea is to take an SVG graphic (image or element) and move it a little bit in the xy plane.
The first example offsets a rectangle (with <feOffset>), then blend the original on top of the offset image (with <feBlend>):

```html
<svg height="120" width="120">
  <defs>
    <filter id="f1" x="0" y="0" width="200%" height="200%">
      <feOffset result="offOut" in="SourceGraphic" dx="20" dy="20" />
      <feBlend in="SourceGraphic" in2="offOut" mode="normal" />
    </filter>
  </defs>
  <rect width="90" height="90" stroke="green" stroke-width="3"
  fill="yellow" filter="url(#f1)" />
</svg>
```
### Code explanation:
The id attribute of the <filter> element defines a unique name for the filter
The filter attribute of the <rect> element links the element to the "f1" filter

### Example 2
Now, the offset image can be blurred (with <feGaussianBlur>):

```html
<svg height="140" width="140">
  <defs>
    <filter id="f2" x="0" y="0" width="200%" height="200%">
      <feOffset result="offOut" in="SourceGraphic" dx="20" dy="20" />
      <feGaussianBlur result="blurOut" in="offOut" stdDeviation="10" />
      <feBlend in="SourceGraphic" in2="blurOut" mode="normal" />
    </filter>
  </defs>
  <rect width="90" height="90" stroke="green" stroke-width="3"
  fill="yellow" filter="url(#f2)" />
</svg>
```
### Code explanation:
The stdDeviation attribute of the <feGaussianBlur> element defines the amount of the blur

### Example 3
Now, make the shadow black:
```html
<svg height="140" width="140">
  <defs>
    <filter id="f3" x="0" y="0" width="200%" height="200%">
      <feOffset result="offOut" in="SourceAlpha" dx="20" dy="20" />
      <feGaussianBlur result="blurOut" in="offOut" stdDeviation="10" />
      <feBlend in="SourceGraphic" in2="blurOut" mode="normal" />
    </filter>
  </defs>
  <rect width="90" height="90" stroke="green" stroke-width="3"
  fill="yellow" filter="url(#f3)" />
</svg>

```

### Code explanation:
The in attribute of the <feOffset> element is changed to "SourceAlpha" which uses the Alpha channel for the blur instead of the entire RGBA pixel





Example 4
Now, treat the shadow as a color:

```html
<svg height="140" width="140">
  <defs>
    <filter id="f4" x="0" y="0" width="200%" height="200%">
      <feOffset result="offOut" in="SourceGraphic" dx="20" dy="20" />
      <feColorMatrix result="matrixOut" in="offOut" type="matrix"
      values="0.2 0 0 0 0 0 0.2 0 0 0 0 0 0.2 0 0 0 0 0 1 0" />
      <feGaussianBlur result="blurOut" in="matrixOut" stdDeviation="10" />
      <feBlend in="SourceGraphic" in2="blurOut" mode="normal" />
    </filter>
  </defs>
  <rect width="90" height="90" stroke="green" stroke-width="3"
  fill="yellow" filter="url(#f4)" />
</svg>
```

### Code explanation:
The <feColorMatrix> filter is used to transform the colors in the offset image closer to black. The three values of '0.2' in the matrix all get multiplied by the red, green and blue channels. Reducing their values brings the colors closer to black (black is 0)


# SVG Gradients - Linear
## SVG Gradients
A gradient is a smooth transition from one color to another. In addition, several color transitions can be applied to the same element.
There are two main types of gradients in SVG:
Linear
Radial

SVG Linear Gradient - <linearGradient>
The <linearGradient> element is used to define a linear gradient.
The <linearGradient> element must be nested within a <defs> tag. The <defs> tag is short for definitions and contains definition of special elements (such as gradients).
Linear gradients can be defined as horizontal, vertical or angular gradients:
Horizontal gradients are created when y1 and y2 are equal and x1 and x2 differ
Vertical gradients are created when x1 and x2 are equal and y1 and y2 differ
Angular gradients are created when x1 and x2 differ and y1 and y2 differ

### Example 1
Define an ellipse with a horizontal linear gradient from yellow to red:
```html
<svg height="150" width="400">
  <defs>
    <linearGradient id="grad1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad1)" />
</svg>
```

Code explanation:
The id attribute of the <linearGradient> tag defines a unique name for the gradient
The x1, x2, y1,y2 attributes of the <linearGradient> tag define the start and end position of the gradient
The color range for a gradient can be composed of two or more colors. Each color is specified with a <stop> tag. The offset attribute is used to define where the gradient color begin and end
The fill attribute links the ellipse element to the gradient


### Example 2
Define an ellipse with a vertical linear gradient from yellow to red:

```html
<svg height="150" width="400">
  <defs>
    <linearGradient id="grad2" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad2)" />
</svg>
```


### Example 3
Define an ellipse with a horizontal linear gradient from yellow to red, and add a text inside the ellipse:
```html
<svg height="150" width="400">
  <defs>
    <linearGradient id="grad3" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:rgb(255,255,0);stop-opacity:1" />
      <stop offset="100%" style="stop-color:rgb(255,0,0);stop-opacity:1" />
    </linearGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad3)" />
  <text fill="#ffffff" font-size="45" font-family="Verdana" x="150" y="86">
  SVG</text>
</svg>

Code explanation:
The <text> element is used to add a text



SVG Gradients - Radial

SVG Radial Gradient - <radialGradient>
The <radialGradient> element is used to define a radial gradient.
The <radialGradient> element must be nested within a <defs> tag. The <defs> tag is short for definitions and contains definition of special elements (such as gradients).
<svg height="150" width="500">
  <defs>
    <radialGradient id="grad1" cx="50%" cy="50%" r="50%" fx="50%" fy="50%">
      <stop offset="0%" style="stop-color:rgb(255,255,255);
      stop-opacity:0" />
      <stop offset="100%" style="stop-color:rgb(0,0,255);stop-opacity:1" />
    </radialGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad1)" />
</svg>
```

### Code explanation:
The id attribute of the <radialGradient> tag defines a unique name for the gradient
The cx, cy and r attributes define the outermost circle and the fx and fy define the innermost circle
The color range for a gradient can be composed of two or more colors. Each color is specified with a <stop> tag. The offset attribute is used to define where the gradient color begin and end
The fill attribute links the ellipse element to the gradient

### Example 2
Define another ellipse with a radial gradient from white to blue:

```html
<svg height="150" width="500">
  <defs>
    <radialGradient id="grad2" cx="20%" cy="30%" r="30%" fx="50%" fy="50%">
      <stop offset="0%" style="stop-color:rgb(255,255,255);
      stop-opacity:0" />
      <stop offset="100%" style="stop-color:rgb(0,0,255);stop-opacity:1" />
    </radialGradient>
  </defs>
  <ellipse cx="200" cy="70" rx="85" ry="55" fill="url(#grad2)" />
</svg>
```
