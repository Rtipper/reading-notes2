# Class 9 Reading Notes - Functional Programming

### Functional Programming
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data
- Pure Functions: It returns the same result if given the same arguments (it is also referred as deterministic) and tt does not cause any observable side effects
- It returns the same result if given the same arguments
- Implement a function that calculates the area of a circle - An impure function would receive radius as the parameter, and then calculate radius * radius * PI
- This is an impure function because it uses a global object that was not passed as a parameter to the function.
- Reading Files - If our function reads external files, it’s not a pure function — the file’s contents can change.
- Random Number Generator - Any function that relies on a random number generator cannot be pure.
- No Observable Side Effects - Examples of observable side effects include modifying a global object or a parameter passed by reference.
- Pure Functions Benefits - Given a parameter A → expect the function to return value B / Given a parameter C → expect the function to return value D
- When data is immutable, its state cannot change after it’s created.
- If you want to change an immutable object, you can’t - Instead, you create a new object with the new value.

### Refactoring JS
- Refactoring code needs a middle ground between speed and accuracy.
- A hash function is used to map a given key to a location in the hash table.
- Return early from functions.
- Cache variables so functions can be read like sentences.
- Check for Web APIs before implementing your own functionality.
- It's important to get your code right the first time because in many businesses there isn't much value in refactoring.
