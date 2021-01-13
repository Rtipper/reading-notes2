# Class 10 Reading Notes - Call Stack & Debugging

### The Callstack
- A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions
- What function is currently being run and what functions are called from within that function, etc.
- When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
- Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
- When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
- If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.
- You always start with an empty Call Stack.
- Whenever we invoke a function, it is automatically added to the Call Stack.
- Once the function has executed all of its code, it is automatically removed from the Call Stack -- like a staging ground.
- Ultimately, the Stack is empty again.
- The JavaScript engine is a single-threaded interpreter comprising of a heap and a single call stack.
-  The browser provides web APIs like the DOM, AJAX, and Timers.
- The call stack is primarily used for function invocation (call).
- Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. 
- It means the call stack is synchronous.
- The understanding of the call stack is vital to Asynchronous programming
- In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue.
- The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.
- Temporarily store: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. 
- This stack frame is a memory location in the stack
- The memory is cleared when the function returns as it is pop out of the stack.
