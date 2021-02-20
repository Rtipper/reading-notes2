# Class 1 Reading Notes

### Array.map
- The `map()` method creates a new array populated with the results of calling a provided function on every element in the calling array.
- `.map()` creates an array from calling a specific function on each item in the parent array.
- In plain english, .map creates an array only after looking at its parent array and the items within it.
- It can have a wide variety of uses when working with arrays.
- It helps your code be more readable as well as iterate through objects, convert strings into arrays or used to render server side via React.
- Ex: <br>

// create a function to use
`const makeSweeter = sweetItem => sweetItem * 2;`

// we have an array
`const sweetArray = [2, 3, 4, 5, 35];`

// call the function we made. more readable
`const sweeterArray = sweetArray.map(makeSweeter);`

`console.log(sweeterArray);`

// Output recieved
`[ 4, 6, 8, 10, 70 ]`

### Array.reduce
- Common termonology to better understand recude is both `accumulator` and `reducer`.
- `accumulatro` is the value that you end up with.
- `reducer` is what action you will perform in order to get one value.
- `reducer` will only return one value and one value only hence the name reduce.
- Using the reduce method, you can do things like flattening an array or changing an object structure.
- Ex: <br>

// this is our initial value i.e. the starting point
`const initialValue = 0;`

// numbers array
`const numbers = [5, 10, 15];`

// reducer method that takes in the accumulator and next item
`const reducer = (accumulator, item) => {
  return accumulator + item;
};`

 we give the reduce method our reducer function and our initial value 
`const total = numbers.reduce(reducer, initialValue)`

### Superagent Example:
- Taken from our 301 Final Project:

`function iHandler(request, response, campArray, weatherData) {
  let location = request.body.city;
  const key = process.env.IQKey;
  let URL = `http://api.airvisual.com/v2/city?city=${location}&state=Washington&country=USA&key=${key}`;
  // console.log(URL)
  superagent.get(URL)
    .then(data => {
      const airQ = data.body.data.current.pollution;
      const yourAir = new Quality(airQ);

      console.log('camp array >>>>>>>>>>>>>>>>>>>>>>>>', campArray);

      let toast = '';

      campArray.forEach(data =>{
        toast += `${data.latLon.lat},${data.latLon.lng}:`;
      })

      toast = toast.substring(0 ,toast.length-1 );
      console.log('toast >>>>>>>>>>>>>>>>>>>>>', toast);

      response.render('pages/results/results-info', { request, response, campArray, weatherData, yourAir, campArrayString: toast });

    });
}`

Taking the `.then` in this case, we are pulling down the information from the API data about and "promising it" into the rendered page.

### Call Backs - Async or Not
- By default, no, but they can be made to be.
- It's when argument of a function is a function.
- A basic example of this is using ForEach.
- Ex: <br>

 `let totalSize = 0;
  items.forEach((item) => {
    totalSize += item.size;
  });
  return totalSize;`


### References:
- https://www.digitalocean.com/community/tutorials/4-uses-of-javascripts-arraymap-you-should-know (digitalocean.com)
- https://www.digitalocean.com/community/tutorials/js-finally-understand-reduce (digitalocean.com)
- https://github.com/Arthur-Lozano/blazingtrails (Blazing Trails -- our 301 final project)
- https://bytearcher.com/articles/does-taking-a-callback-make-a-function-asynchronous/#:~:text=Simply%20taking%20a%20callback%20doesn,argument%20but%20are%20not%20asynchronous.&text=It%20iterates%20over%20each%20item%20and%20calls%20the%20function%20once%20per%20item.
