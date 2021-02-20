# Class 1 Reading Notes

### Array.map
- The map() method creates a new array populated with the results of calling a provided function on every element in the calling array.
- `.map()` creates an array from calling a specific function on each item in the parent array.
- In plain english, .map creates an array only after looking at its parent array and the items within it.
- It can have a wide variety of uses when working with arrays.
- Ex: <br>
// create a function to use
` const makeSweeter = sweetItem => sweetItem * 2; `

// we have an array
` const sweetArray = [2, 3, 4, 5, 35]; `

// call the function we made. more readable
` const sweeterArray = sweetArray.map(makeSweeter); `










### References:
- https://www.digitalocean.com/community/tutorials/4-uses-of-javascripts-arraymap-you-should-know (digitalocean.com)
- 
