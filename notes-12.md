# Class 12 Reading Notes

### Chart.js, Canvas
-  Chart.js is a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page.
- Different types of charts can be created by downloading and changing the HTML of the Chart.js files.
- Once you’ve mastered the basics here, you’ll discover that there are tons of options listed in the documentation.

### Canvas
- A canvas looks like the img element, with the only clear difference being that it doesn't have the src and alt attributes.
- The canvas element has only two attributes, width and height, which are optional and can also be set using DOM properties.
- The canvas will initially be 300 pixels wide and 150 pixels high.
- The canvas element differs from an img tag in that, like for video, audio, or picture elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.
- Setting Fallback Content: insert the alternate content inside the canvas element. Browsers that don't support canvas will ignore the container and render the fallback content inside it.
- As a consequence of the way fallback is provided, unlike the img element, the canvas element requires the closing tag (</canvas>)
- The canvas element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown.
- The canvas will be initially blank. To display something, a script first needs to access the rendering context and draw on it. 
- The canvas element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context.

### Drawing Shapes with Canvas
- Unlike SVG, canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines).
- "fillRect(x, y, width, height)" draws a rectangle.
- "strokeRect(x, y, width, height)" draws a rectangular outline.
- "clearRect(x, y, width, height)" Clears the specified rectangular area, making it fully transparent.
- Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.
- The fillRect() function draws a large black square 100 pixels on each side. The clearRect() function then erases a 60x60 pixel square from the center, and then strokeRect() is called to create a rectangular outline 50x50 pixels within the cleared square.

### Styles and Colors
- fillStyle = color sets the style used when filling shapes.
- strokeStyle = color sets the style for shapes' outlines.
- Color is a string representing a CSS color, a gradient object, or a pattern object. By default, the stroke and fill color are set to black (CSS color value #000000).

### Drawing Text
- fillText(text, x, y [, maxWidth]) fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
- strokeText(text, x, y [, maxWidth]) strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
- font = value the current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.
- textAlign = value text alignment setting. Possible values: start, end, left, right or center. The default value is start.
- textBaseline = value baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.
- direction = value directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

