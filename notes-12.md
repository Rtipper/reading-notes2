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
