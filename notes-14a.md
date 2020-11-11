# Class 14a Reading Notes

## CSS Transforms

### Transform Syntax
- The transform property comes in two different settings, two-dimensional and three-dimensional. 
- Each of these come with their own individual properties and values.
- The transform property followed by the value: -webkit-transform: scale(1.5); / -moz-transform: scale(1.5); / -o-transform: scale(1.5); / transform: scale(1.5); 
- These are placed inside of a div in the given example.
- The transform property includes multiple vendor prefixes to gain the best support across all browsers.
- The un-prefixed declaration comes last to overwrite the prefixed versions, should a browser fully support the transform property.
### 2d Transforms
- Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. 
- Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. 
- Three-dimensional transforms work on both the x and y axes, as well as the z axis.
- Three-dimensional transforms help define not only the length and width of an element, but also the depth.
- The rotate value provides the ability to rotate an element from 0 to 360 degrees.
- Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. 
- The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.
- Ex: "<figure class="box-1">Box 1</figure>" / ".box-1 { transform: rotate(20deg); }"
- Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.
- It is possible to scale only the height or width of an element using the scaleX and scaleY values. 
- The scaleX value will scale the width of an element while the scaleY value will scale the height of an element.
- The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.
- Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.
- Skew is used to distort elements on the horizontal axis, vertical axis, or both. 
- The syntax is very similar to that of the scale and translate values. 
- Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis.

## Transitions and Animations

### Transitions
- With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
- Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes.
- for a transition to take place, an element must have a change in state, and different styles must be identified for each state. 
- The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.
- There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay.
### Transitional Property
- The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. 
- By default, all of the properties within an element’s different states will be altered upon change. 
- However, only the properties identified within the transition-property value will be affected by any transitions.
- If multiple properties need to be transitioned they may be comma separated within the transition-property value.
### Transitional Properties
- It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point.
- Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. 
- The display property, for example, may not be transitioned as it does not have any midpoint.
### Transition Duration
- The duration in which a transition takes place is set using the transition-duration property. 
- The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). 
- These timing values may also come in fractional measurements, .2s for example.
- When transitioning multiple properties you can set multiple durations, one for each property.
- As with the transition-property property value, multiple durations can be declared using comma separated values. 
- The order of these values when identifying individual properties and durations does matter.

## 8 Popular CCS3 Transitions **(http://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)**
- Fade In: Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover.
- Change Color: Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them. Now, we just set the div’s class to “color” and specify the color we want in our CSS.
- Grow & Shrink: To grow an element, you used to have to use its width and height, or its padding. Set your div’s class to “grow” and then add this code to your style block.
- Shrinking an element is as simple as growing it. To enlarge an element we specify a value greater than 1, to shrink it, we specify a value less than 1.
- Rotate Elements: Give your div the class “rotate” and add the following to your CSS: -webkit-transform: rotateZ(-30deg); / -ms-transform: rotateZ(-30deg); / transform: rotateZ(-30deg);
- Square to Circle: Give your div the class “circle” and add border-radius:50%;
- 3D Shadow: Give your div the class “threed” and then add: box-shadow: / 1px 1px #53a7ea, / 2px 2px #53a7ea, / 3px 3px #53a7ea; / -webkit-transform: translateX(-3px); / transform: translateX(-3px);
- Swing: This animation simply moves the element left and right, now all we need to do is apply it.
- Inset Border: Give your div the class “border” and add box-shadow: inset 0 0 0 25px #53a7ea;

## Button Animations (CodePen)
- https://codepen.io/retyui/pen/ByoaXV 

## CSS3 Keyframes Animations (CodePen)
- https://codepen.io/akshaychauhan/pen/oAfae

## 404 (CodePen)
- https://codepen.io/kieranfivestars/pen/MYdQxX

## CSS Bounce Animation (CodePen)
- https://codepen.io/dp_lewis/pen/gCfBv
                
               
        
        
