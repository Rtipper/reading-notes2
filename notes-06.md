# Reading Note Class 6

### Chpt 3 - Object Literals
- In an object, varibales become knonw as properties: If a variable is part of an object, it is called a property. Properties te ll us about the object, such as the name of a hotel or the number of rooms it has. Each individual hotel might have a different name and a different number of rooms.
- In an object, functions become known as methods: If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object. For example, you can check how many rooms are available by subtracting the number of booked rooms from the total number of rooms.
- Like variables and named functions, properties and methods have a name and a va lue. In an object, that name is called a key.
- An object cannot have two keys with the same name. This is because keys are used to access their corresponding values.
- The value of a property can be a string, number, Boolean, array, or even another object. The va lue of a method is always a function.
ex:
var hotel = {                         ------
name: 'Quay',                              -
rooms: 40,                                 - Properties (these are variables)
booked: 25,                                -
gym: true,                                 -
roomTypes: ['twin', 'double', 'suite'],  ---

checkAvailability: function() {       ------
  return this.rooms - this.booked;         - Method (this is a function)
  }                                   ------
};

- Above you can see a hotel object. The object contains the following key/value pairs:
- name - string
- rooms - number
- booked - number
- gym - Boolean
- roomTypes - array
- checkAvailability - function

- Literal notation is the easiest and most popular way to create objects.
- You access the properties or methods of an object using dot notation. You can also access properties using square brackets
ex:
var hotelName = hotel.name;
var roomsFree - hotel.checkAvailability();

- Functions allow you to group a set of related statements together that represent a single task.
- Functions can take parameters (informatiorJ required to do their job) and may return a value.
- An object is a series of variables and functions that represent something from the world around you.
- In an object, variables are known as properties of the object; functions are known as methods of the object.
- Web browsers implement objects that represent both the browser window and the document loaded into the browser window.
- JavaScript also has several built-in objects such as
- String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.
- Arrays and objects can be used to create complex data sets (and both can contain the other).

### Chpt 5 - Document Object Model (DOM)
- The browser represents the page using a DOM tree.
- DOM trees have four types of nodes: document nodes, element nodes, attribute nodes, and text nodes.
- You can select element nodes by their id or class attributes, by tag name, or using CSS selector syntax.
- Whenever a DOM query can return more than one node, it will always return a Nade List.
- From an element node, you can access and update its content using properties such as textContent and inner HTML or using DOM manipulation techniques.
- An element node can contain multiple text nodes and child elements that are siblings of each other.
- In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).
- Browsers offer tools for viewing the DOM tree.
