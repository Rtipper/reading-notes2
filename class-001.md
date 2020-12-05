# 301 Class 01 - Reading Notes

## Responsive Web Design

- Mobile growth has exploded onto the internet scene
- The growth of mobile Internet usage is also far out pacing that of general Internet usage growth.
- In the UK there are more mobile phones than people, and should trends continue mobile Internet usage will surpass that of desktop Internet usage within the year.
- The industry response to this question has become responsive web design, also known as RWD.
- Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.
- Responsive web design is focused around providing an intuitive and gratifying experience for everyone. 
- Desktop computer and cell phone users alike all benefit from responsive websites.
- Responsive and adaptive web design are closely related, and often transposed as one in the same.
- Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change.
- With responsive design websites continually and fluidly change based on different factors, such as viewport width, while adaptive websites are built to a group of preset factors.
- Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users.
- Mobile websites can be extremely light but they do come with the dependencies of a new code base and browser sniffing, all of which can become an obstacle for both developers and users.
- Currently the most popular technique lies within responsive web design, favoring design that dynamically adapts to different browser and device viewports, changing layout and content along the way.
### Flexible Layouts
- Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media.
- The first part, flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
- Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. 
- Reason being, the viewport height and width continually change from device to device.
- The formula is based around taking the target width of an element and dividing it by the width of it’s parent element.
### Media Queries
- Media queries were built as an extension to media types commonly found when targeting and including styles.
- Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example.
### Mobile First
- The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.
- The operating belief behind mobile first design is that a user on a mobile device, commonly using a smaller viewport, shouldn’t have to load the styles for a desktop computer only to have them over written with mobile styles later.
- Before too long, the majority of Internet consumption will be done on a mobile device.
### Flexible Media
- As viewports begin to change size media doesn’t always follow suit
- Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.
- One quick way to make media scalable is by using the max-width property with a value of 100%. Doing so ensures that as the viewport gets smaller any media will scale down according to its containers width.

## All About Floats

- Float is a CSS positioning property. 
- In page layout programs, the boxes that hold the text can be told to honor the text wrap, or to ignore it
- Ignoring the text wrap will allow the words to flow right over the image like it wasn’t even there.
- This is the difference between that image being part of the flow of the page (or not)
- Floated elements remain a part of the flow of the web page. This is distinctly different than page elements that use absolute positioning.
- Absolutely positioned page elements are removed from the flow of the webpage, like when the text box in the print layout was told to ignore the page wrap.
- Absolutely positioned page elements will not affect the position of other elements and other elements will not affect them, whether they touch each other or not.
- There are four valid values for the float property: Left and Right float elements those directions respectively. None (the default) ensures the element will not float and Inherit which will assume the float value from that elements parent element.
- Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.
- Floats are also helpful for layout in smaller instances.
- Float’s sister property is clear.
- An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.


