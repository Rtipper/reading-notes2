# Class 03 Reading Notes - Flexbox & Templating

### JS Templating
- Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.
- The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
- The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.
- Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything.
- It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops.
- mustache.js is an implementation of the mustache template system in JavaScript.
- It is often considered the base for JavaScript templating. And, since mustache supports various languages, we don’t need a separate templating system on the server side.
- Mustache is NOT a templating engine.
- Mustache is a specification for a templating language. In general, we would write templates according to the Mustache specification, and it can then be compiled by a templating engine to be rendered to create an output.
- If you intend you use mustache with Node and Express, you can use mustache-express.
- Mustache Express lets you use Mustache and Express together easily.

### Flexbox
- Items: Boxes inside a container.
- Containers: Box that holds the items, or smaller boxes.
- display: This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
- order: By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container.
- flex-direction: This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns (row, row-reverse, column, column-reverse)
- flex-grow: This defines the ability for a flex item to grow if necessary. It accepts a unitless value that serves as a proportion. It dictates what amount of the available space inside the flex container the item should take up.
- flex-wrap: By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property (nowrap, wrap, wrap-reverse).
- flex-shrink: This defines the ability for a flex item to shrink if necessary.
- flex-flow: This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.
- flex-basis: This defines the default size of an element before the remaining space is distributed. It can be a length (e.g. 20%, 5rem, etc.) or a keyword.
- justify-content: This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. 
- flex: his is the shorthand for flex-grow, flex-shrink and flex-basis combined. 
- align-self: This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.
- align-items: This defines the default behavior for how flex items are laid out along the cross axis on the current line. 
- align-content: This aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.


