# Class 12 Reading Note - Components

### EJS Partials
- Partials work like functions -- they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in.
- Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.
- Create additional files in ejs which will contain only the HTML for what you are manipulating.
- Once you have your partials defined, we can use them in our home.ejs and post.ejs templates.
- In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters (you could change these delimiters if you really wanted to) -- STRAWBERRIES
- Including a partial in EJS is quite straightforward. You use <%- include( PARTIAL_FILE ) %> where the partial file is relative to the template you use it in.
- The <%- %> tags allow us to output the unescaped content onto the page (notice the -).
- This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc.
- Creating and including partials is very straightforward with EJS and adapting them to code you already have.
