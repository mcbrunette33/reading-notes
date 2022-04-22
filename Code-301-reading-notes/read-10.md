# Read 10

## JavaScript Call Stack

- The call stack is used for function invocation (call).
- these functions are executed one at a time, from top to bottom.
- The call stack is synchronous.
- A stack is a data structure that uses Last in, First Out(LIFO) principle to temp store and mangae function calls.
- The last functino that gets pushed into the stack, is the first to be popped out when the function returns.

## Stack Overflow

- Stack overflow occurs when here is a recursive function(a function that calls itself without an exit point.
- function callMyself() { callMyself();} callMyself();
- The call Myself() will run until the browser throws a "Maximum call size exceeded". This is stack overflow.

## Keys

- only do one thing at a time.
- Code execution is synchronous.
- functions calls/invocation creates a stack frame that occupies a temp memory.
- It works as a LIFO- last in, first out data structure.

## Javascript Error Message && Debugging

- Error messages appear in your console.
- Declare vars before any declaration is made.

## Syntax Errors

- syntax erros occure when something cannot be parsed.

## Range Errors

- when an object has an invalid length.
- an array cannot have a negative length.

## Type Errors

- these type of errors show up when the types (number, string) you are not trying to use or access are incompatible, like accessing a property in an indefined type of varible.
- var foo = {} foo.bar // undefined.
- making sure something exist before trying to accesss it.

## Debugging

- use console.log() on the variables you want to check.
- use chrome developer tools and open the file you want to debug.
- use debugger statement in your code in the line you want to break.

## Handling Errors

- use a try catch statement to find errors
- wrap the function code block in a try {} catch {} and console.long(err).